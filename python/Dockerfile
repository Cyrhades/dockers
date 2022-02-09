FROM ubuntu:latest

LABEL author.lastname="LECOMTE" author.firstname="Cyril"

RUN apt-get update && apt-get install -y python python-pip wget
ADD hello.py /home/hello.py

WORKDIR /home