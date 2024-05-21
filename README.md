# web-hing

## 소개

**web-hing** 프로젝트는 Java 17(azul-17)과 Spring Boot 3.2.5를 사용하여 Web API 백엔드 서버를 구축하는 템플릿을 제공합니다. 

## 목표
프로젝트의 목표는 정형화된 응답 모델과 공통 컨트롤러를 통해 개발자가 비즈니스 로직(service)에만 집중할 수 있도록 하여, 부가적인 코드 작성의 필요성을 최소화하는 것입니다. 또한, properties 설정을 최대한 활용하여 설정 관리에 대한 부담을 줄이고, 백엔드 서비스를 공장에서 찍어내듯이 쉽게 템플릿화하는 것을 목표로 합니다.

## What Hing?
**Hing**의 의미는 "Happiness In Now and Goodness"로, 현재의 행복과 선함을 추구하는 마음을 담고 있습니다.

## 기능

- **정형화된 응답 모델**: 일관된 응답 형식을 제공하여 클라이언트와의 통신을 쉽게 만듭니다.
- **공통 컨트롤러**: 공통된 기능을 제공하는 컨트롤러를 통해 중복 코드를 줄입니다.
- **비즈니스 로직 집중**: 서비스 로직에만 집중할 수 있도록 지원하여 개발 생산성을 높입니다.
- **properties 설정 활용**: 설정 관리의 편의성을 높여 개발자가 설정 변경에 신경 쓸 필요가 없도록 합니다.

## 기술 스택

- Java 17 (Azul Zulu)
- Spring Boot 3.2.5

## 설치 및 실행 방법

### 사전 요구 사항

- Java 17 설치 (Azul Zulu 권장)
- Maven

### 클론 및 빌드

```bash
git clone https://github.com/yourusername/web-hing.git
cd web-hing
./mvnw clean install  # 또는 ./gradlew build
```

### 프로젝트 구조
``` 
web-hing/
 ├── src/
 │   ├── main/
 │   │   ├── java/
 │   │   │   └── com/
 │   │   │       └── example/
 │   │   │           └── webhing/
 │   │   │               ├── controller/
 │   │   │               ├── service/
 │   │   │               ├── model/
 │   │   │               └── WebHingApplication.java
 │   │   └── resources/
 │   │       ├── application.properties
 │   │       └── static/
 │   └── test/
 │       ├── java/
 │       │   └── com/
 │       │       └── example/
 │       │           └── webhing/
 │       │               └── WebHingApplicationTests.java
 │       └── resources/
 ├── .gitignore
 ├── README.md
 └── pom.xml
``` 

# Server settings
server.port=8080

# Data source settings
spring.datasource.url=jdbc:mysql://localhost:3306/webhing
spring.datasource.username=root
spring.datasource.password=password

# Hibernate settings
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

# Logging
logging.level.org.springframework=INFO



# 연락처
프로젝트에 대해 궁금한 점이 있거나 제안사항이 있다면 언제든지 연락주세요:

Email: tlsehdgml159@gmail.com\
GitHub: hidonghee