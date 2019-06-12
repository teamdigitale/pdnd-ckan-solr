# Data & Analytics Framework (DAF) CKAN

Ckan solr is a specific component used by CKAN in the context of the Data Analytics Framework (DAF) project. Apache Solr is a highly reliable, scalable and fault tolerant software component, providing distributed indexing, replication and load-balanced querying, automated failover and recovery, centralized configuration and more. Solr powers the search and navigation features of many of the world's largest internet sites.

## What is the Data & Analytics Framework (DAF)?

More informations about the DAF can be found on the [Digital Transformation Team website](https://teamdigitale.governo.it/it/projects/daf.htm)

## Tools references

The tools referenced in this repository are

* [CKAN](https://ckan.org/)
* [Apache Solr](https://lucene.apache.org/solr/)

## Project components

* **CKAN** 2.6.2 is the current version chose for the project. The tool is included in this repository, available [here](https://github.com/teamdigitale/daf-ckan)

* **Solr** version 6.2 (packaged for CKAN and with some customizations)

* **PostgreSQL** version 10.8 is certified to work with the current CKAN distribution. PostgreSQL is pulled in as a dependency from the official Docker repositories (see Docker documentation below).

* **Redis** version 5.0.5 is certified to work with the current CKAN distribution. Redis is automatically pulled in as a dependency from the official Docker repositories (see Docker documentation below).

## How to build this version of Solr and test it as part of CKAN

This specific version of Solr is distributed and consumed in a form of Docker container.

The container can be build using the `dockerfile` in the root of this repository.

Docker-compose is used to build a fully-functional test environment (build the CKAN container and download pre-packaged dependencies - including solr). Instructions can be found in the [CKAN repository](https://github.com/teamdigitale/daf-ckan).

## How to contribute

Contributions are welcome. Feel free to open issues and submit a pull request at any time!

This is a temporary repository, still maintained because consumed by the production DAF environment. Anyway, an ongoing development work is moving on [here](https://github.com/italia/dati-ckan-docker).
