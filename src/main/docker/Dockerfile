FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD eureka-service-0.0.1-SNAPSHOT.jar eureka-service.jar
RUN sh -c 'touch /eureka-service.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /eureka-service.jar" ]
