FROM openjdk:11-jre-slim

LABEL author.lastname="LECOMTE" author.firstname="Cyril"
ENV USER burpsuite
ENV HOME /home/${USER}
ENV APP https://portswigger-cdn.net/burp/releases/download?product=community&version=2021.12.1&type=Jar

RUN apt-get update && apt-get install openjdk-11-jdk --no-install-recommends -y sudo software-properties-common wget openssl libxext6 libxrender1 libxtst6 libxi6
RUN useradd -d ${HOME} -m ${USER} &&  passwd -d ${USER} && adduser ${USER} sudo

USER ${USER}
WORKDIR ${HOME}

RUN sudo mkdir /burp && sudo chown -R ${USER}:${USER} /burp && wget -q -O /burp/burpsuite.jar ${APP} && mkdir -p ${HOME}/.java/.userPrefs/burp/ 
RUN sudo addgroup burp && sudo adduser ${USER} burp
CMD java -jar /burp/burpsuite.jar