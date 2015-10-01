## Java Dockerfile


This repository contains **Dockerfile** of [Java](https://www.java.com/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/emilianobonassi/oracle-java/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [ubuntu:14.04](https://registry.hub.docker.com/_/ubuntu)


### Docker Tags

`emilianobonassi/oracle-java` provides multiple tagged images:

* `latest` (default): Oracle Java 8 JDK (alias to `8`)
* `6`: Oracle Java 6 JDK
* `7`: Oracle Java 7 JDK
* `8`: Oracle Java 8 JDK

For example, you can run a `Oracle Java 8` container with the following command:

    docker run -it --rm emilianobonassi/oracle-java:8 java -version


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/emilianobonassi/oracle-java/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull emilianobonassi/oracle-java`

   (alternatively, you can build an image from Dockerfile: `docker build -t="emilianobonassi/oracle-java" github.com/emilianobonassi/java`)


### Usage

    docker run -it --rm emilianobonassi/oracle-java

#### Run `java`

    docker run -it --rm emilianobonassi/oracle-java java

#### Run `javac`

    docker run -it --rm emilianobonassi/oracle-java javac
