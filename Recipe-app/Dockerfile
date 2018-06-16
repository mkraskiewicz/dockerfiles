FROM centos
RUN yum install -y java

VOLUME /tmp
ADD /recipe-app-0.0.1-SNAPSHOT.jar recipe-app.jar
RUN sh -c 'touch /recipe-app.jar'
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom","-jar","/recipe-app.jar"]