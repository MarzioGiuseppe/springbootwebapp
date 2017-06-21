FROM openjdk
MAINTAINER Marzio Parenti <marzio.parenti@gmail.com>

COPY environment /etc/environment

VOLUME /tmp

ADD springbootwebapp.jar myapp.jar
RUN sh -c 'touch /myapp.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/myapp.jar"]
