# Docker Compose Configuration for Hadoop, Hive, Spark, PostgreSQL, Cassandra, and Hue

This repository provides a configuration for running a multi-service environment, based on [Big Data Europe's repositories](https://github.com/big-data-europe), consisting of: Hadoop, Hive, Spark, PostgreSQL, Cassandra, and Hue. 

It allows developers to easily set up and manage these services within Docker containers.

## Hadoop Services
- Namenode
- Datanode
- Resourcemanager
- Hive Server
- Hive Metastore
- Hive Metastore PostgreSQL

## Spark Services
- Spark Master
- Spark Worker 1

## Databases:
- PostgreSQL
- Cassandra

## Other Services:
- Python 3.9
- Hue

## Volumes:
- namenode
- datanode
- pg_data
- cassandra_data

Please note that this `docker-compose.yml` file assumes the presence of a `hadoop-hive.env` file in the same directory, which contains the necessary environment variables for the services. 
Make sure to provide the required configurations in the `hadoop-hive.env` file before running the Docker Compose command.

To start the services, navigate to the directory containing the `docker-compose.yml` file and run the following command:
    
    docker-compose up -d
    
