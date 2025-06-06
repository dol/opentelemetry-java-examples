FROM eclipse-temurin:17-jre

COPY build/libs/app.jar build/agent/opentelemetry-javaagent.jar build/agent/opentelemetry-javaagent-extension.jar /

CMD ["-javaagent:/opentelemetry-javaagent.jar", "-Dotel.javaagent.extensions=/opentelemetry-javaagent-extension.jar", "-jar", "/app.jar"]
ENTRYPOINT ["java"]
