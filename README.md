안녕하세요, 백엔드 개발자 **Junfe(김준철)** 입니다.

주로 **Java / Spring Boot / MySQL / Docker / AWS**를 사용해
결제·수납·매출·정산 도메인의 백엔드 서비스를 설계·개발·운영해 왔습니다.

**운영 안정성과 데이터 정합성**을 핵심 가치로,
장애 원인 분석부터 DB 구조 개선까지 실질적인 개선을 만드는 백엔드 개발자를 지향합니다.

---

## 🧱 Experience

- 📸 **서북(Seobuk) – Photoism CMS 백엔드 개발자** (2025.04 ~ 2025.11)
  - 글로벌 포토이즘 서비스 CMS 백엔드 개발·운영 (한국·일본·중국 등 다국가 리전)
  - 피크 시간대 결제 집중 + 대용량 엑셀 다운로드로 발생한 **CMS OOM 장애** 분석 및 해결
    - 애플리케이션 로그 기반 원인 특정 → JVM `-Xmx` 리전별 상향 조정 (EC2 스펙 대비 ~50%)
    - 엑셀 생성 방식 **XSSF → SXSSF 스트리밍 전환**으로 힙 메모리 점유 최소화
  - 리전별 분산 매출 데이터를 통합한 **글로벌 매출·정산 대시보드 설계 및 ETL 파이프라인 구축**
    - MySQL Stored Procedure + Event Scheduler 기반 일 배치, 7일 Upsert로 데이터 정합성 확보
    - **정산 리드타임 5일 → 2일 (약 60% 단축)**
  - 앱 2.0 전환 과정 CMS 1.0 ↔ CMS 2.0 쿠폰 검증·사용 처리 API 연동
  - Jenkins 기반 국가·리전별 배포 Job 운영, New Relic APM 도입

- 🎓 **창의와탐구 – 백엔드 개발자** (2021.09 ~ 2025.04)
  - 학원관리 LMS 백엔드 전반 개발·운영 (풀스택 단독 개발, Java 8 / Spring Boot / MyBatis / JSP)
  - **온라인 결제 PG 전환** (이니시스 → 먼쓸리페이) 및 네이버페이 연동
    - 화면·서버 이중 레이어 중복결제 방지 로직 구현, 전국 100여 개 가맹 학원 적용
  - **수강·결제 DB 구조 개편** — 청구서 테이블 제거, 수강-매출 중심 구조로 간소화
    - 이수·휴회·반이동 등 수강 변동 케이스 범용 금액 계산 로직 설계 및 구현
    - 수강 변동 관련 DB 수정 CS 요청 **약 80% 감소**

- 🏛 **G2B Platform** (2025 ~ 진행 중, 외주 개발)
  - 정부 조달(나라장터) 계약 데이터를 수집·통합·분석하는 풀스택 플랫폼
  - raw → flat → grouped 다단 ETL 파이프라인, 보고서·대시보드·엑셀 다운로드
  - **Claude Code + Jira MCP** 기반 AI 에이전트 개발 워크플로우 운영
    - 작업 계획 컨펌 → 티켓 자동 생성 → 코드 구현·PR → 본인 리뷰·머지 승인
  - AWS EC2 + RDS + Docker Compose + Nginx 배포 환경 직접 구축

- 🩺 **JW메디칼 – 의료장비 필드 엔지니어** (2019.01 ~ 2020.10)
  - 병원 현장 MRI/CT 장비 설치·유지보수·장애 대응
  - 현장 로그·에러코드 기반 원인 분석, 신속한 문제 해결 역량 확보

---

## 🛠 Tech Stack

**Backend**
- Java 8 / 17 / 21, Spring Boot, Spring MVC / WebFlux
- Spring Data JPA, MyBatis, Spring Security, OAuth2
- Gradle, Maven

**Database & Infra**
- MySQL, MariaDB
- AWS EC2 / RDS / S3
- Docker, Docker Compose, Nginx
- Jenkins, New Relic

**Frontend (보조)**
- Vue 3, Vite, JavaScript, jQuery, JSP

**Etc**
- Apache POI (SXSSF 스트리밍 엑셀)
- Google Sheets API
- Git, GitHub / Bitbucket, Jira
- Claude Code + MCP 기반 AI 에이전트 개발

---

## 📂 Featured Projects

- 🏛 **G2B Platform** *(진행 중)*
  정부 조달 계약 데이터를 수집·적재·분석하는 Spring Boot 기반 풀스택 플랫폼
  `Java 21 / Spring Boot 3.3 / JPA / MyBatis / MySQL / Vue 3 / Docker / AWS`

---

## 📫 Contact

- Email: `ogum0405@hanmail.net`
- GitHub: [@JunFe23](https://github.com/JunFe23)
- Blog: [junfe5.tistory.com](https://junfe5.tistory.com)

---

<details>
<summary>English version 🌐</summary>

### Hi there 👋

I'm **Junfe (Juncheol Kim)**, a backend developer based in Seoul, Korea.

I mainly work with **Java, Spring Boot, MySQL, Docker and AWS**,
building backend services focused on **operational stability and data integrity**
across payment, billing, settlement and data pipeline domains.

#### Experience

- 📸 **Backend Developer at Seobuk – Photoism CMS** (Apr ~ Nov 2025)
  - Developed and operated the backend for Photoism CMS across multi-country regions (KR/JP/CN)
  - Diagnosed and resolved **CMS OOM incidents** caused by peak-time payment load + large Excel exports
    - Identified root causes via application logs → adjusted JVM `-Xmx` per region (~50% of EC2 memory)
    - Replaced XSSF with **SXSSF streaming** to minimize heap usage during large downloads
  - Designed and built a **global revenue & settlement dashboard with ETL pipeline**
    - MySQL Stored Procedure + Event Scheduler batch, daily 7-day Upsert for data integrity
    - **Reduced settlement lead time from 5 days to 2 days (~60% improvement)**
  - Handled CMS 1.0 ↔ 2.0 coupon validation/usage API integration during app 2.0 migration

- 🎓 **Backend Developer at Changui & Tamgu** (Sep 2021 ~ Apr 2025)
  - Full-cycle backend development for an LMS (solo, full-stack)
  - **PG migration** (Inicis → Monthleypay) with dual-layer duplicate payment prevention
  - **DB restructuring** for enrollment-payment data — removed invoice tables, simplified to enrollment-sales flow
    - Designed universal fee calculation logic for all enrollment change cases
    - **~80% reduction** in DB modification support requests

- 🏛 **G2B Platform** (2025 ~, freelance)
  - Full-stack platform for collecting and analyzing government procurement contract data
  - Built raw → flat → grouped multi-stage ETL pipeline, dashboard, and Excel export
  - Operates with **Claude Code + Jira MCP** AI agent workflow (plan → ticket → code → review → merge)

#### Tech

- Backend: Java, Spring Boot, Spring MVC/WebFlux, JPA, MyBatis, Spring Security
- DB/Infra: MySQL, AWS EC2/RDS, Docker, Docker Compose, Nginx, Jenkins, New Relic
- Tools: Apache POI (SXSSF), Google Sheets API, Git, GitHub/Bitbucket

Thanks for visiting! 🙌

</details>
