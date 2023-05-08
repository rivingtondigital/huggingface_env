from jupyter/scipy-notebook:latest

USER root
RUN apt-get -qq update
RUN apt-get install -y vim
RUN apt-get install -y pip
RUN apt-get install -y curl
RUN curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
RUN apt-get install -y git-lfs

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
USER jovyan
