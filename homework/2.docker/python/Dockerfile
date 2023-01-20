FROM ubuntu:latest
MAINTAINER Mik 'mik_h@mail.com'
RUN apt-get update -y
RUN apt-get install -y python-pip build-essential
RUN apt-get update -y && apt-get upgrade -y pip && pip install --upgrade pip
COPY . /app
WORKDIR /app 
RUN pip install -r requirements.txt
ENTRYPOINT ['python']
CMD ['app.py']