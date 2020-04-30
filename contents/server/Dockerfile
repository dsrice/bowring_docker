FROM python:3.7
ENV PYTHONUNBUFFERED 1
RUN mkdir /code
RUN apt-get update
WORKDIR /code
ADD requirement.txt /code/
RUN pip install -r requirement.txt
ADD . /code/
WORKDIR /code/bowringserver
RUN apt-get install -y default-mysql-client

EXPOSE 8000