FROM docker
RUN apk add --update maven
RUN apk add --update unzip
RUN apk add --update openjdk8
ENV JAVA_HOME /usr/lib/jvm/java-1.8-openjdk
ENV PATH ${PATH}:${JAVA_HOME}/bin
COPY --from=docker/buildx-bin /buildx /usr/libexec/docker/cli-plugins/docker-buildx
CMD javac -version
