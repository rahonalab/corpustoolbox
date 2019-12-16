Docker-compose yaml file for doing corpus linguistics.

## Features
- based upon official Python Docker image
- NLP Python modules: NLTK, treetaggerwrapper, opus-tools
- automatic building of CWB tools (latest version)

## Installation
1. Edit .env and secrets.env to fit your needs (see below for details).
2. `docker-compose build`
3. `docker-compose run corpustoolbox bash`
4. Happy corpus linguistics!

## Configuration
Before starting, you have to modify two files: .env and secrets.env

### secrets.env
This file is read by containers: you just have to set LOCALTIME.

### .env
This file is read by docker-compose; you need to set the following variables:

| Variable | Description & Usage |
| -------- | ------------------- |
| FIRSTNAME | your project name |
| DOMAINNAME | your domain name |
| DATA | CWB corpus data on local filesystem |
| REGISTRY | CWB registry on local filesystem |
| WORK | working place on local filesystem  |




