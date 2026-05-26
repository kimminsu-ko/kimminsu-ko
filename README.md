# 김민수 | Backend Developer

문제를 기능 단위로만 보지 않고, 인증·권한·실시간 이벤트·배포 운영까지 이어지는 구조로 설계하는 개발자입니다.

낯선 도메인에서도 먼저 흐름과 제약을 파악하고, 반복되는 문제를 유지보수 가능한 구조로 정리하는 데 집중합니다. 최근에는 Spring Boot 기반 도메인 설계, Redis/WebSocket 기반 실시간 처리, Docker/Jenkins/nginx 기반 운영 자동화, MSA 이벤트 흐름 설계를 경험하고 있습니다.

[![Email](https://img.shields.io/badge/Email-tkatnsdl1996%40daum.net-0A66C2?style=flat-square)](mailto:tkatnsdl1996@daum.net)
[![GitHub](https://img.shields.io/badge/GitHub-kimminsu--ko-181717?style=flat-square&logo=github)](https://github.com/kimminsu-ko)

## Focus

| Area | Keywords |
| --- | --- |
| Backend | Java, Spring Boot, JPA, Spring Security, JWT/OAuth2 |
| Realtime / Event | Redis, WebSocket, FCM, MQTT, Redis Streams, Socket.IO |
| Infra / Ops | Docker Compose, Jenkins, nginx, Cloudflare, Prometheus, Grafana, Loki |
| Data / AI | MySQL, PostgreSQL, TimescaleDB, Python, Flask, PyTorch, OpenAI API |
| Frontend | React, TypeScript, Vue, Vue-i18n |

## Featured Projects

| Project | Role | What I Built | Stack |
| --- | --- | --- | --- |
| [AIEMS](https://github.com/kimminsu-ko/AIEMS) | Team Lead / Full | MSA 기반 마이크로그리드 EMS 실시간 모니터링 및 AI 예측 시스템. MQTT, Redis Streams, Socket.IO를 연결해 telemetry 수집부터 상태 처리, 예측, 운영 화면까지 이어지는 이벤트 흐름을 설계했습니다. | Python, Flask, Redis Streams, MQTT, Socket.IO, PostgreSQL, TimescaleDB, Docker, AWS EC2 |
| [TIKIT](https://github.com/kimminsu-ko/TIKIT) | Team Lead / Backend | NFC 기반 스마트 명함 교환 및 출입 권한 관리 플랫폼. OAuth2/JWT 인증, Redis 기반 토큰 검증, NFC 출입증, WebSocket/FCM 알림 흐름을 설계했습니다. | Spring Boot, JPA, Redis, WebSocket, FCM, OAuth2, JWT, Arduino |
| [SSAFYMaker](https://github.com/kimminsu-ko/SSAFYMaker) | Infra / Full | Phaser 기반 SSAFY 육성 게임과 운영 자동화 프로젝트. 단일 EC2에서 STG/PROD/OPS/AUTH 스택을 분리하고 Jenkins, n8n, nginx, Cloudflare, Grafana 기반 운영 구조를 구성했습니다. | TypeScript, Phaser, Spring Boot, Keycloak, Docker Compose, Jenkins, nginx, Grafana |
| [SilkRoad](https://github.com/kimminsu-ko/silkroadfront) | Frontend | 외국인 대상 국내 여행 리뷰 플랫폼. Vue-i18n 기반 다국어 구조, API 응답 매핑, Naver Map API 전환을 통해 외국인 사용자 경험을 개선했습니다. | Vue, Vue-i18n, JavaScript, Naver Map API, CSS |

## Problem Solving

- 조회가 많은 도메인에서는 변경 감지 기준을 두고, 불필요한 재조회 비용을 줄이는 구조를 고민했습니다.
- 인증과 권한은 기능 뒤에 붙이는 처리가 아니라, 도메인 경계와 함께 설계해야 하는 기준으로 다룹니다.
- 실시간 상태 변화는 polling보다 이벤트 흐름을 먼저 검토하고, producer/consumer 책임을 명확히 나누려 합니다.
- 운영 도구는 외부에 필요한 endpoint만 열고, UI는 whitelist로 보호하는 방식으로 노출 범위를 분리했습니다.
- 협업 혼선은 문서를 더 쓰는 것보다, Swagger나 이벤트 계약처럼 모두가 같은 기준을 보게 만드는 구조로 줄이려 합니다.

## Project Direction

현재는 백엔드 중심으로 서비스를 설계하되, 배포 이후 운영과 장애 대응까지 고려하는 방향으로 성장하고 있습니다. 기능 구현에서 끝내지 않고, 서비스가 오래 유지될 수 있는 구조를 만드는 개발자가 되는 것이 목표입니다.
