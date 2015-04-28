FROM chosenken/jdk-8
MAINTAINER chosenken@gmail.com

ENV MVN_VERSION 3.3.1

RUN curl -sSL http://archive.apache.org/dist/maven/maven-3/$MVN_VERSION/binaries/apache-maven-$MVN_VERSION-bin.tar.gz | tar xzf - -C /usr/share \
	&& mv /usr/share/apache-maven-$MVN_VERSION /usr/share/maven \
	&& ln -s /usr/share/maven/bin/mvn /usr/bin/mvn

ENV MAVEN_HOME /usr/share/maven

CMD ["mvn"]
