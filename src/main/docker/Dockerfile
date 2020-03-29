FROM openjdk:11

ENV SPRING_OUTPUT_ANSI_ENABLED=ALWAYS \
    JAVA_OPTS="" \
    SERVER_PORT=80

CMD echo "The application will start..." && \
    java ${JAVA_OPTS} -Djava.security.egd=file:/dev/./urandom -jar /app.jar --server.port=$SERVER_PORT
    
ADD target/*.jar /app.jar