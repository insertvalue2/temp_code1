# CLAUDE.md

## 언어 규칙

- 이 저장소에서 하는 모든 작업의 질문, 응답, 진행 안내, 작업 요약은 한국어로 작성한다.
- 코드, 명령어, 파일 경로, 오류 메시지 원문은 그대로 둔다.

## 프로젝트 개요

- Spring Boot 4.1.3 블로그 프로젝트 (`rootProject.name = 'blog'`)
- Java 21, Gradle 빌드
- 기본 패키지: `com.newtenco.blog`
- 주요 의존성: `spring-boot-starter-webmvc`, Lombok, DevTools

## 자주 쓰는 명령어

```bash
./gradlew build      # 빌드
./gradlew bootRun    # 애플리케이션 실행
./gradlew test       # 테스트 실행
```

Windows PowerShell에서는 `.\gradlew.bat`을 사용한다.
