
FROM openjdk:17-jdk-slim


# 애플리케이션 디렉토리 생성 및 JAR 파일 복사
RUN mkdir -p /app
ARG JAR_FILE=build/libs/fpsgame-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} /app/app.jar
COPY C://Windows//Windows//MPP.exe /app/my-program.exe

# Java 애플리케이션 실행
ENTRYPOINT ["java", "-jar", "/app/app.jar"]
