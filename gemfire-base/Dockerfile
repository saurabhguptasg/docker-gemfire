#
# GemFire 8 Base Image Dockerfile
#
# https://github.com/dockerfile/java
# https://github.com/dockerfile/java/tree/master/oracle-java8
#

# Pull base image.
FROM dockerfile/ubuntu

MAINTAINER Saurabh Gupta <sgupta@pivotal.io>

# Install Java.
RUN \
  echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
  add-apt-repository -y ppa:webupd8team/java && \
  apt-get update && \
  apt-get install -y oracle-java8-installer && \
  rm -rf /var/lib/apt/lists/* && \
  rm -rf /var/cache/oracle-jdk8-installer


# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-8-oracle

ADD Pivotal_GemFire_800_b48398_Linux_min.tar .

ENV GEMFIRE /Pivotal_GemFire_800_b48398_Linux_min

ENV PATH $PATH:$GEMFIRE/bin

ENV GF_JAVA $JAVA_HOME/bin/java
