# 베이스 이미지 설정
FROM openjdk:21-jdk-slim

# 작업 디렉토리 생성
WORKDIR /app

# 소스 코드 복사
COPY . /app

# Gradle 빌드 실행
RUN ./gradlew build

# JAR 파일 실행
ENTRYPOINT ["java", "-jar", "build/libs/app.jar"]
