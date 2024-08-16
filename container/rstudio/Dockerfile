FROM ghcr.io/rocker-org/rstudio:4

RUN apt-get update && apt-get upgrade -y &&\
apt-get install python3-pip -y

COPY ./container/rstudio/requirements.txt /tmp/

RUN pip3 install -r /tmp/requirements.txt

ENV DISABLE_AUTH=true