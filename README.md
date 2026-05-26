# 안녕하세요, 김민수입니다.

백엔드를 중심으로 서비스를 만들고, 배포 이후 운영까지 이어지는 구조를 고민합니다.

기능을 빠르게 붙이는 것도 중요하지만, 저는 그 기능이 어떤 도메인 안에서 동작하는지, 인증과 권한은 어디서 막아야 하는지, 장애가 생겼을 때 어디까지 영향을 줄지 먼저 보는 편입니다.

최근에는 Spring Boot 기반 도메인 설계, Redis/WebSocket 기반 실시간 처리, Docker/Jenkins/nginx 기반 배포 자동화, MSA 이벤트 흐름 설계를 경험하고 있습니다.

[![Email](https://img.shields.io/badge/Email-tkatnsdl1996%40daum.net-0A66C2?style=flat-square)](mailto:tkatnsdl1996@daum.net)
[![GitHub](https://img.shields.io/badge/GitHub-kimminsu--ko-181717?style=flat-square&logo=github)](https://github.com/kimminsu-ko)

## 제가 주로 보는 것

- 요구사항을 도메인 단위로 나누고, 유지보수하기 쉬운 구조로 정리하는 것
- 인증, 권한, 토큰, 접근 제어처럼 서비스의 기준이 되는 흐름을 설계하는 것
- 실시간 상태 변화나 알림을 이벤트 흐름으로 자연스럽게 연결하는 것
- 배포 이후에도 확인하고 복구할 수 있는 운영 구조를 만드는 것
- 협업 과정에서 기준이 흔들리지 않도록 API 명세와 문서로 맞추는 것

## Projects

### [AIEMS](https://github.com/kimminsu-ko/AIEMS)
MSA 기반 마이크로그리드 EMS 실시간 모니터링 및 AI 예측 시스템입니다.

- MQTT, Redis Streams, Socket.IO를 연결해 telemetry 수집부터 운영 화면까지 이어지는 이벤트 흐름을 설계했습니다.
- 서비스별 producer/consumer 책임을 나누고, EC2 부하 특성에 맞춰 배치 구조를 조정했습니다.
- AI가 직접 장비를 제어하지 않고 예측과 운영 판단 보조 역할만 하도록 경계를 분리했습니다.

`Python` `Flask` `Redis Streams` `MQTT` `Socket.IO` `PostgreSQL` `TimescaleDB` `Docker`

### [TIKIT](https://github.com/kimminsu-ko/TIKIT)
NFC 기반 스마트 명함 교환 및 출입 권한 관리 플랫폼입니다.

- 팀장으로 백엔드 구조와 인증/권한 흐름을 설계했습니다.
- OAuth2/JWT, Redis 기반 토큰 검증, NFC 출입증, WebSocket/FCM 알림 흐름을 연결했습니다.
- Swagger와 문서화를 통해 프론트와 백엔드의 API 해석 차이를 줄였습니다.

`Spring Boot` `JPA` `Redis` `WebSocket` `FCM` `OAuth2` `JWT` `Arduino`

### [SSAFYMaker](https://github.com/kimminsu-ko/SSAFYMaker)
Phaser 기반 SSAFY 육성 게임과 운영 자동화 프로젝트입니다.

- 단일 EC2에서 STG, PROD, OPS, AUTH 스택을 Docker Compose 단위로 분리했습니다.
- Jenkins와 n8n으로 배포 및 알림 흐름을 자동화했습니다.
- nginx와 Cloudflare로 외부 노출 범위를 나누고, Grafana/Loki로 운영 상태를 볼 수 있게 구성했습니다.

`TypeScript` `Phaser` `Spring Boot` `Keycloak` `Docker Compose` `Jenkins` `nginx` `Grafana`

### [SilkRoad](https://github.com/kimminsu-ko/silkroadfront)
외국인 대상 국내 여행 리뷰 플랫폼 프론트엔드입니다.

- Vue-i18n 기반 다국어 구조를 정리했습니다.
- 백엔드 API 응답 구조와 프론트 데이터 매핑을 맞춰 렌더링 오류를 줄였습니다.
- 외국인 사용자에게 주소가 더 잘 전달되도록 지도 API를 검토하고 전환했습니다.

`Vue` `Vue-i18n` `JavaScript` `Naver Map API` `CSS`

## Tech Stack

`Java` `Spring Boot` `JPA` `Spring Security` `JWT/OAuth2`  
`Redis` `WebSocket` `FCM` `MQTT` `Redis Streams` `Socket.IO`  
`Docker Compose` `Jenkins` `nginx` `Cloudflare` `Prometheus` `Grafana` `Loki`  
`Python` `Flask` `PostgreSQL` `TimescaleDB` `React` `TypeScript` `Vue`

## 방향성

지금은 백엔드 중심으로 서비스를 설계하되, 배포 이후 운영과 장애 대응까지 함께 보는 개발자로 성장하고 있습니다. 기능 구현에서 끝내지 않고, 팀이 오래 다룰 수 있는 구조를 만드는 것이 목표입니다.
