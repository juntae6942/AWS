# AWS Computing
고가용성은 장애가 5분미만인 서비스를 의미한다.

## 클라우드 컴퓨팅이란?
- 온디맨드로 서비스 액세스
- 필요에 따라 컴퓨팅 리소스 프로비저닝(공급, 할당)
- 사용한만큼만 비용 지불  

## 주요 이점
- 거대한 규모의 경제로 얻게 되는 이점
- 용량 추정 불필요
- 속도 및 민첩성 향상
- 비용 절감 목표 실현
- 몇 분 만에 전세게에 배포

가용영역 - 하나 이상의 데이터 센터  
리전 - 가용영역 3개 이상  
POP(Point of Presence, 엣지 로케이션) - 콘텐츠 캐시 영역

## 서비스 관리
관리 콘솔(Management Console)
명령줄 인터페이스(CLI, Command Line Interface)
소프트웨어 개발 키트(SDK, Software Development Kit)

## 공동 책임 모델 다이어그램
고객(클라우드 내부의 보안 담당)  
- 고객 데이터   
- 플랫폼, 애플리케이션, 자격 증명 및 액세스 관리
- 운영체제, 네트워크, 방화벽 구성
- 클라이언트 측 데이터, 암호화 및 데이터 무결성 인증
- 서버 측 암호화(파일 시스템 및 데이터)
- 네트워킹 트래픽 보호  

AWS(클라우드 자체의 보안 담당)
- 소프트웨어
- 컴퓨팅, 저장, 데이터베이스, 네트워킹
- 하드웨어/AWS 글로벌 인프라
- 리전, 가용영역, 엣지 로케이션

## IAM(Identity and Access Management)
1단계 - AWS 계정 만들기  
2단계 - 첫 번째 IAM 사용자를 생성 후 다른 사용자 생성 권한을 제공(Admin 계정 만들기)
IAM 사용자 - MFA 요구

### IAM 정책 
- 서비스 및 리소스 권한을 부여하거나 거부하는 문서
- JSON 요소
  - Version: 정책 언어의 버전을 정의
  - Effect: 액세스를 허용할지 또는 거부할지 여부를 지정
  - Action: 허용하거나 거부해야 하는 작업의 유형을 설명
  - Resource: 정책문에서 다루는 객체를 지정

## 컴퓨팅 서비스
### 인스턴스
  - EC2(Elastic Compute Cloud)
    - 가상 서버 프로비저닝
    - 시작할 때 먼저 AMI(Amazon Machine Image)를 선택
      - AMI 요소
        - 운영체제
        - 스토리지 매핑
        - 아키텍처 유형
        - 시작 권한
        - 추가 소프트웨어 애플리케이션
    - 지정한 AMI를 루트 디바이스에 볼륨에 복사
  - 범용
  - 컴퓨팅 최적화
  - 메모리 최적화
  - 가속 컴퓨팅
  - 스토리지 최적화
### 컨테이너
  - ECS(Elastic Container Service)
  - EKS(Elastic Kubernetes Service)
    - MSA 설계를 위해 Kubernetes를 쓰기 시작하는 단계
      - 사용자가 많아질 때
      - 서비스 로직의 규모가 커지면서 장애가 발생하게 될 때
  - Fargate
### 서버리스
  - 관리 할 필요가 없다는 의미, 서버가 없는게 아님
  - Lambda


# AWS Networking
# AWS Storage
# Database
# Monitoring, LoadBalancing 및 Scaling
# 강좌 요약