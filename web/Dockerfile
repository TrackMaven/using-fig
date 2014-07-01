# Our base image is Ubuntu 13.04
FROM stackbrew/ubuntu:raring
# Install any updates
RUN apt-get -y update
# Ensure python is installed and postgres drivers.
RUN apt-get install -y python python-pip python-psycopg2

ADD requirements.txt /code/requirements.txt
RUN pip install -r /code/requirements.txt
WORKDIR /code