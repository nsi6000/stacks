FROM alpine:latest
#docker image build -t python-smack:latest .

WORKDIR /smack

#COPY . /app

RUN apk update
RUN apk add vim
RUN apk add git
RUN apk add wget
RUN apk add gcc


#Python
#Python standard library: os, gzip, curses, csv, json, pprint, unittest, pydoc, queue, re, uuid, tkinter, time, sqlite3, dbm.
RUN apk add python3
RUN apk add py3-pip #pip
RUN pip3 install Faker #faker
RUN pip3 install msgpack #messagepack
RUN pip3 install pprint
#RUN pip3 install coala-bears #coala linter
RUN pip3 install proselint #proselint
RUN pip3 install pylint
RUN pip3 install jsonschema #JSON schema validator

#SMACK
RUN pip3 install pymongo #mongodb
RUN pip3 install cassandra-driver #Cassandra / ScyllaDB
#RUN pip3 install pyspark #Spark
RUN pip3 install confluent-kafka #Kafka




# Make port 80 available to the world outside this container
EXPOSE 5000

# Define environment variable
ENV NAME World

# Run app.py when the container launches
#CMD ["python", "app.py"]

