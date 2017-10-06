FROM registry.cn-beijing.aliyuncs.com/kv/oracle-jdk:8.0
VOLUME /tmp
ADD config-server-1.0.jar /app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
