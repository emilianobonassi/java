#
# Oracle Java 8 Dockerfile
#
# https://github.com/emilianobonassi/java
# https://github.com/emilianobonassi/java/tree/master/oracle-java8
#

# Pull base image.
FROM ubuntu:14.04

ENV DEBIAN_FRONTEND noninteractive

# Install Java.
RUN \
  apt-get update -y && \
  apt-get install software-properties-common -y && \
  add-apt-repository -y ppa:webupd8team/java && \
  apt-get update

RUN \
  echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
  apt-get install -y oracle-java8-installer     && \
  rm -rf /var/lib/apt/lists/*                   && \
  rm -rf /var/cache/oracle-jdk8-installer

# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-8-oracle

# Define default command.
CMD ["bash"]
