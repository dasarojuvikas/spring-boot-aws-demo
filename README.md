# AWS Application

Simple Spring Boot REST API for deployment on AWS EC2.

## API

GET /hello

Response:

hello spring boot

## Run locally

```bash
mvn spring-boot:run
```

Open:

http://localhost:8080/hello

## Build JAR

```bash
mvn clean package
```

## Run JAR

```bash
java -jar target/aws-application-0.0.1-SNAPSHOT.jar
```

## AWS EC2

1. Install Java 17 on the EC2 instance.
2. Allow inbound TCP port 8080 in the EC2 Security Group.
3. Copy the JAR to EC2.
4. Run:

```bash
java -jar aws-application-0.0.1-SNAPSHOT.jar
```

5. Access:

http://YOUR_EC2_PUBLIC_IP:8080/hello
