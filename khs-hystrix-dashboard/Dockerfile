FROM java:8
VOLUME /tmp
ADD target/khs-hystrix-dashboard-1.0.0-SNAPSHOT.jar app.jar
RUN bash -c 'touch /app.jar'
EXPOSE 7979
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom", "-jar","/app.jar"]