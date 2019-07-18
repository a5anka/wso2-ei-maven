FROM maven:3.6.0-jdk-8

RUN useradd -ms /bin/bash -u 1000 wso2ei

RUN apt-get update && apt-get install -y --no-install-recommends \
		gcc \
		gcc-multilib \
	&& rm -rf /var/lib/apt/lists/*

COPY cacerts /docker-java-home/jre/lib/security/cacerts
