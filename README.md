# 🚀 template-springboot-web
> Spring Boot Web 프로젝트 개발을 위한 기본 스타터 템플릿
## 📌 Project Overview
이 프로젝트는 **Java 21**과 **Spring Boot 4.0.3**을 기반으로 하며, 빠른 초기 설정을 위해 주요 의존성과 YAML 설정이 포함되어 있습니다.

---

## 🛠 Tech Stack & Environment

### Project Metadata
| 항목 | 내용 |
| :--- | :--- |
| **Project** | Gradle - Kotlin |
| **Language** | Java 21 |
| **Spring Boot** | 4.0.3 |
| **Group** | `com.template` |
| **Artifact** | `web` |
| **Package Name** | `com.template.web` |
| **Packaging** | Jar |
| **Configuration** | YAML (`application.yml`) |

### Dependencies
* **Spring Web**: MVC를 사용하여 RESTful 애플리케이션을 빌드하기 위한 핵심 의존성
* **Spring Boot DevTools**: 코드 변경 시 자동 재시작 등 개발 편의 기능 제공
* **Spring Data JPA**: Hibernate를 이용한 데이터 액세스 계층 추상화
* **H2 Database**: 개발 및 테스트를 위한 인메모리 데이터베이스
* **Lombok**: Annotation을 통해 Getter, Setter, 생성자 등을 자동 생성

---

## ⚙️ Configuration
기본 설정은 `src/main/resources/application.yml`에서 관리합니다.

```yaml
spring:
  datasource:
    url: jdbc:h2:mem:testdb
    driver-class-name: org.h2.Driver
    username: sa
    password:
  h2:
    console:
      enabled: true
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
