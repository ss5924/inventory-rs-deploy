# 🛫 MyMachine
재고 관리 시스템


# 📃 프로젝트 정보
- 제작기간 : 2024.06.27 ~ 06.29


# 📚 사용 기술
### 1. Back-End
- Java
- Spring Boot
- Spring Data JPA
- Spring Cloud
- MariaDB
- redis
- kafka


### 2. CI/CD
- Docker
- Docker registry
- Nexus
- Jenkins


# 📊 ERD & Structure

### 1. ERD
![erd](https://github.com/user-attachments/assets/91108042-104d-4627-bafa-7483f3b51efa)

### 2. Structure
![시스템백엔드구조도 drawio](https://github.com/user-attachments/assets/d4588399-deb4-4401-98b8-5f875754a78e)


<!-- # 🔑 핵심기능-->


# 📕 기타 자료
### 1. 요청서
- 시스템 요청서.pdf 확인 

### 2. 관련 리포지토리
- https://github.com/ss5924/inventory-rs-deploy
- https://github.com/ss5924/inventory-rs-gateway
- https://github.com/ss5924/inventory-rs-machine-service
- https://github.com/ss5924/inventory-rs-loc-service
- https://github.com/ss5924/inventory-rs-config

### 2. 프로젝트 목적 및 후기
- 이 프로젝트의 목표는 실무에서 사용할 수 있는 백엔드 시스템을 설계하고 운영하는 것
- Spring Boot를 기반으로 RESTful API를 설계하고, JPA와 MariaDB를 사용해 데이터베이스를 구축하여 데이터 관리와 성능을 최적화함
- Kafka를 활용해 실시간 데이터 처리와 메시지 전달을 구현하고, Redis를 적용해 캐싱 전략을 도입하여 처리 속도를 개선함
- Docker를 사용해 애플리케이션을 컨테이너화하여 독립적인 개발 환경을 구현했고, Docker Registry를 통해 이미지를 효율적으로 관리함
- Spring Cloud를 통해 마이크로서비스 아키텍처를 구성하고 서비스 간의 통신을 효율적으로 처리하여 확장성과 유연성을 확보
- 개발 환경에서는 Maven을 통해 의존성 관리를 하고, Git과 Jenkins를 사용해 CI/CD 파이프라인을 구축함
- Nexus를 통해 아티팩트 관리를 최적화하여 배포 프로세스의 효율성을 극대화함
- 최종적으로, 실무와 유사한 환경을 구현한다는 목표를 달성할 수 있었음
