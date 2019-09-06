FROM java:8
MAINTAINER demo scl@sina.com
VOLUME /tmp
ADD eurekaserver-0.0.1-SNAPSHOT.jar eurekaserver.jar
RUN sh -c 'touch /eurekaserver.jar'
EXPOSE 8520
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /eurekaserver.jar" ]
