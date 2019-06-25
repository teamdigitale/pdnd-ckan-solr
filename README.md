# CKAN Solr for Piattaforma Digitale Nazionale Dati (PDND), previously DAF

Ckan solr is a specific component used by CKAN in the context of the PDND project. Apache Solr is a highly reliable, scalable and fault tolerant software component, providing distributed indexing, replication and load-balanced querying, automated failover and recovery, centralized configuration and more. Solr powers the search and navigation features of many of the world's largest internet sites.

## What is the PDND (previously DAF)?

PDND stays for "Piattaforma Digitale Nazionale Dati" (the Italian Digital Data Platform), previously known as Data & Analytics Framework (DAF).

You can find more informations about the PDND on the official [Digital Transformation Team website](https://teamdigitale.governo.it/it/projects/daf.htm).

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

Contributions are welcome. Feel free to [open issues](./issues) and submit a [pull request](./pulls) at any time, but please read [our handbook](https://github.com/teamdigitale/daf-handbook) first.

## License

Copyright (c) 2019 Presidenza del Consiglio dei Ministri

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
