ARG MAVEN_VERSION=3.5.4-jdk-8
FROM maven:$MAVEN_VERSION

LABEL vendor="Infinity Refactoring" \
      git.repository="https://github.com/InfinityRefactoring/docker-maven" \
      authors="Thomás Sousa Silva (ThomasSousa96)"

RUN apt-get update \
      && apt-get install gnupg2 \
      && apt-get install git \
      && apt-get install git-flow

COPY settings.xml /root/.m2/