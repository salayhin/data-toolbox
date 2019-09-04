FROM jupyter/scipy-notebook

USER root

RUN mkdir /notebooks
RUN mkdir .ssh

WORKDIR  /notebooks

COPY ./requirements.txt /home/requirements.txt

RUN apt-get update 
RUN apt-get install libpq-dev python-dev

#RUN pip install psycopg2 pymysql google-cloud-bigquery paramiko sshtunnel mlflow=1.0.0

RUN apt-get install -y python-dev libmysqlclient-dev libpq-dev
RUN pip install -r /home/requirements.txt
