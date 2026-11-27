# CLAUDE.md

## 언어 규칙

- 이 저장소에서 하는 모든 작업의 질문, 응답, 진행 안내, 작업 요약은 한국어로 작성한다.
- 코드, 명령어, 파일 경로, 오류 메시지 원문은 그대로 둔다.

## 작업 목적

- 기준 교안: https://insertvalue2.github.io/class_book_rest_api_v1 (직접 만든 스프링 부트 REST API 강의 교안, 「스프링부트4로배우는 REST API」)
- 사용자가 교안의 장과 절 순서대로 강의를 따라가며 코드를 직접 작성하고, 실행과 테스트로 교안 내용이 실제로 동작하는지 확인한다.

## 역할 분담

- 코드 작성과 실행은 사용자가 직접 한다. Claude는 요청이 없으면 코드를 작성하거나 파일을 수정하지 않는다.
- Claude는 사용자의 질문에 답한다. 주된 질문은 다음 세 가지다.
  - 개념적 오류: 교안의 설명이 틀렸거나 오해를 부르는 부분
  - 코드 오류: 컴파일 오류, 실행 오류, 테스트 실패, 버전 차이로 인한 문제
  - 안 좋은 코드: 동작은 하지만 관례에 어긋나거나 수강생에게 나쁜 습관을 들일 수 있는 코드
- 답할 때는 해당 장의 교안 원문과 저장소의 실제 코드를 함께 확인하고 근거를 밝힌다.
- 질문에서 교안과 실제 동작이 다른 부분이 확인되면 `PROGRESS.md`의 표에 기록하자고 제안한다.

## 진행 기록

- 진행 상황은 `PROGRESS.md`에 장별로 기록한다.

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
