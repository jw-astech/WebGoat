FROM openjdk:8-jre
VOLUME /tmp
RUN cd /root; mkdir -p .webgoat
ADD webgoat-server-8.0-SNAPSHOT.jar webgoat.jar
RUN sh -c 'touch /webgoat.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/webgoat.jar"]