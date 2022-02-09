FROM ubuntu:20.04
LABEL author.lastname="LECOMTE" author.firstname="Cyril"

# Installation de python et curl
RUN apt-get update && apt-get install -y python curl
# Installation de pip (systeme de package de Python)
RUN curl https://raw.githubusercontent.com/Cyrhades/pip/master/get-pip.py -o get-pip.py && python get-pip.py
# On se place dans notre répertoire de travail
WORKDIR /home