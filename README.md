# 개요
web-Bubble 프로젝트

## 개발 환경
- Java : jdk 21
- IntelliJ : 2021.03 이상 (Java 17버전 대응 가능)
- Spring boot : 3.3.7
- Gradle : 8.10.2

## 포함
- Mybatis
- Redis
  - cluster
  - queue
- Cassandra
- AWS
  - s3

## 사용시 참고사항
- package는 프로젝트에 맞게 수정하여 사용할 것
  - 현재 co.dearu.web.bubble
  - 끝에 꼭 api를 붙일 필요는 없음. 프로젝트 성격에 맞게 수정.
  - 예) co.dearu.abcde.api, co.dearu.abcde.scheduler
- db, redis는 endpoint별로 패키지 구분
  - redis의 경우 master, slave 클래스 구분

## 테스트 클래스 생성 규칙
- test/java/co/dearu/test/api 폴더 하위에 epic 이슈명으로 폴더 생성
  - 예) LPM-001 > LPM_001  (dash는 폴더,파일명으로 사용 불가)
- 해당 폴더 하위에 하위이슈명으로 테스트 클래스 생성
  - 예) LPM-001-LPM-101 > LPM_001_LPM_101_Controller_Test

  