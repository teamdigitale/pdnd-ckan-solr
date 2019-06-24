# Data & Analytics Framework (DAF) CKAN

Ckan solr is a specific component used by CKAN in the context of the Data Analytics Framework (DAF) project. Apache Solr is a highly reliable, scalable and fault tolerant software component, providing distributed indexing, replication and load-balanced querying, automated failover and recovery, centralized configuration and more. Solr powers the search and navigation features of many of the world's largest internet sites.

## What is the Data & Analytics Framework (DAF)?

More informations about the DAF -a.k.a. Piattaforma Digitale Nazionale Dati (PDND)- can be found on the [Digital Transformation Team website](https://teamdigitale.governo.it/it/projects/daf.htm)

## Tools references

The tools referenced in this repository are

* [CKAN](https://ckan.org/)
* [Apache Solr](https://lucene.apache.org/solr/)

## Project components

* **CKAN** version 2.6.4, available [here](https://github.com/teamdigitale/daf-ckan).

* **Solr** version 6.2, packaged for CKAN and with some customizations. What's inside this repository.

* **PostgreSQL** version 10.1, modified for CKAN. The container is available [here](https://hub.docker.com/r/geosolutionsit/dati-ckan-docker/tags). The image is tagged `postgresql-10.1`.

* **Redis** version 5.0.5. Redis is automatically pulled in as a dependency from its [official Docker repository](https://hub.docker.com/_/redis).

## How to build this version of Solr and test it as part of CKAN

This specific version of Solr is distributed and consumed in a form of Docker container.

The container can be built using the `dockerfile` in the root of this repository.

Docker-compose is used to build a fully-functional test environment (build the CKAN container and download pre-packaged dependencies, including Solr).

Instructions can be found in the [CKAN repository](https://github.com/teamdigitale/daf-ckan).

## How to contribute

Contributions are welcome. Feel free to open issues and submit a pull request at any time!

This is a temporary repository, still maintained because consumed by the production DAF environment. Anyway, an ongoing development work is moving on [here](https://github.com/italia/dati-ckan-docker).
