# 취미 및 프로필 인증 기반 프리미엄 데이팅 앱 MVP 구축 — 제안 분석 로그

> 생성일: 2026-06-09
> 공고 URL: https://www.wishket.com/project/155926/

## 1. 공고 파싱 결과

```yaml
job:
  title: "취미 및 프로필 인증 기반 프리미엄 데이팅 앱 MVP 구축"
  category: "개발/디자인/기획 · 웹/안드로이드/iOS · 중개·매칭 플랫폼"
  budget_range: "20,000,000원 (실시간: 최저 1,800만 / 평균 1,900만 / 최고 2,000만)"
  duration: "60일"
  tech_stack:
    - "Flutter 또는 React Native"
    - "Firebase 또는 Supabase"
    - "FCM (푸시 알림)"
    - "실시간 채팅"
  description: |
    취미 및 프로필 인증을 기반으로 신뢰할 수 있는 이성을 추천받고,
    양방향 호감 표시를 통해 매칭 및 대화를 나눌 수 있는 프리미엄 데이팅 앱 MVP.
  requirements:
    - "소셜 로그인 및 휴대폰 본인 인증"
    - "프로필 등록 및 관리 (사진/정보)"
    - "취미 및 성향 키워드 선택"
    - "추천 피드 (스와이프 또는 리스트)"
    - "기본 필터 (나이/지역/취미)"
    - "좋아요 및 매칭 신청/확인"
    - "매칭 성공 화면 (양방향 호감 일치)"
    - "1:1 실시간 채팅 (Firebase/Supabase)"
    - "푸시 알림 (FCM)"
    - "관리자 승인 시스템 (인증 사진 심사, 가입 승인)"
    - "관리자 백오피스 (웹 또는 DB 직접 관리)"
  client_questions: []
  deadline: "2026-06-23"
  job_post_url: "https://www.wishket.com/project/155926/"
  urls: []
  images: []
  deliverables:
    - "앱 설치 파일 및 각 스토어 등록"
    - "소스 코드 원본"
    - "관리자 매뉴얼"
  qualifications:
    - "iOS 및 Android 앱 구축 경험"
  preferred:
    - "Firebase 또는 Supabase 기반 기술 스택 및 실시간 채팅 구현 경험"
  contract_eligibility:
    - "개인 또는 팀 / 개인사업자 가능 / 법인사업자 가능"
```

## 2. URL/이미지 분석

- 공고에 포함된 외부 URL: 없음 (위시켓 공고 URL 외 참고 링크 미제공)
- 공고에 첨부된 이미지: 없음
- 별도 기획 문서(제안요청서)가 존재한다고 명시되어 있으나 공고 본문에는 미첨부 → 계약 후 상세 기획 협의 전제

## 3. 실현 가능성 분석 (내부용)

### 프로젝트 유형
- 모바일 앱 (Flutter/RN) — **조건부 가능** (+20% 버퍼)
- 실시간 채팅 + 푸시 — Firebase/Supabase BaaS 활용으로 난이도 완화 (전용 실시간 서버 불필요)

### 기본 공수 산정 (AI 보조 없이)
- 기획/설계: 8 M/D
- Figma 디자인: 10 M/D
- FE Flutter (앱 9개 핵심 기능): 35 M/D
- BE (Firebase/Supabase + 관리자 백오피스): 20 M/D
- QA/배포 (스토어 등록 포함): 10 M/D
- **Total raw: 83 M/D**

### AI 절감률 적용
- 기획: 8 × 0.65 = 5.2
- Figma: 10 × 0.85 = 8.5
- FE: 35 × 0.35 = 12.25
- BE: 20 × 0.45 = 9.0
- QA: 10 × 0.5 = 5.0
- **Subtotal: ~40 M/D**

### 버퍼 적용 + 달력 일수 변환
- 모바일 +20%: 40 × 1.2 = ~48 M/D
- 달력 일수: 48 × (7/5) = ~67일

### 클라이언트 예상 vs 산정
- 클라이언트 예상: 60일
- 효율적 산정: ~67일 (+7일, 약 10% 초과 → **20% 이내**)
- **판정**: 60일 그대로 제안 (스코프 동결 + 단계별 납품 전략)
- BaaS(Firebase/Supabase) 활용으로 실시간/푸시 구현 리스크가 낮아 60일 내 출시 충분히 가능

## 4. 포트폴리오 매칭

### 매칭 점수 (요구사항 4축 기준: 기술 40 / 도메인 30 / 기능 20 / 규모 10)
| Project | 기술 스택 | 도메인 | 기능 | 규모 | 합계 |
|---------|----------|-------|------|------|-----|
| **Connectin** | Flutter 풀스택 (35) | 매칭 플랫폼 (30) | 프로필·매칭·1:1 메시징 (20) | 12 MS·3개월 (10) | **95** |
| **Calendar Share** | Flutter+Firebase+Supabase (40) | 소셜 앱 (20) | 실시간 채팅·7종 FCM·좋아요 (20) | MVP (5) | **85** |
| **Fortune App** | Flutter+Firebase (35) | B2C 라이프스타일 (15) | SSO·포인트·게이미피케이션 (15) | 3개월 단독 (10) | **75** |
| DayStarter | Flutter+NestJS (30) | 게이미피케이션 (10) | 가상재화·결제 (10) | 3년 (10) | 60 |
| Harmony Link | Flutter+NestJS (25) | 헬스케어 (10) | 실시간·알림·관리 (15) | 6개월 (10) | 60 |

### 최종 추천 3개 (사용자 요청으로 Calendar Share → Harmony Link 교체)
1. **Connectin** — 프로필 기반 매칭·1:1 메시징 도메인 직접 경험 (가장 직접적 유사)
2. **Harmony Link** — Next.js RBAC 관리자 백오피스 + FCM 실시간 푸시 + Flutter 소셜 로그인 (관리자 승인 시스템·알림 직접 대응)
3. **Fortune App** — Flutter B2C 단기 양대 마켓 출시 패턴 + 소셜 로그인 (60일 일정 근거)

## 5. 최종 제안 요약

- **지원 금액**: 17,000,000원 (VAT 별도)
  - 산정 근거: 클라이언트 예상 금액 2,000만원 × 85% (사용자 조정) = 17,000,000원
- **지원 기간**: 60일 (계약 체결 직후 즉시 착수)
  - 산정 근거: 클라이언트 예상 60일과 일치, 내부 산정 ~67일이나 20% 이내 → 스코프 동결 + 단계별 납품으로 60일 매칭
- **핵심 제안 포인트**:
  1. Connectin (프로필 기반 매칭 + 1:1 메시징 + Flutter 양대 마켓) 매칭 플랫폼 도메인 직접 경험 전이
  2. Harmony Link (Next.js RBAC 관리자 백오피스 + FCM 실시간 푸시 + Flutter 소셜 로그인) 관리자 승인 시스템·알림 직접 대응
  3. Fortune App (Flutter B2C 3개월 풀패키지 출시 + SSO) 60일 MVP 출시 일정의 실현 근거
  4. 신뢰 기반 인증 흐름(휴대폰 본인 인증 + 관리자 인증 사진 심사 승인) MVP 단계부터 견고하게 구성
  5. 취미·성향 키워드·매칭 로그 정형화 적재로 추천 고도화 확장 대비

## 6. 최종 산출물 (8단계 출력 전문)

### 제안서 사이트 URL
- **https://proposal-router.claude-ai-b27.workers.dev/proposal-hobby-verified-dating-app-mvp/**
- GitHub: https://github.com/Blue-Verse/proposal-hobby-verified-dating-app-mvp

### 지원 금액 (복사용)
```
17,000,000원
```
산정: 클라이언트 예상 금액 2,000만원 × 85% (사용자 조정) = 17,000,000원 (VAT 별도)

### 지원 기간 (복사용)
```
60일
```
계약 체결 직후 즉시 착수, iOS/Android 동시 출시까지 60일

### 클라이언트 질문 답변
- 공고에 클라이언트 작성 질문 없음 → 해당 없음

### 지원 내용 (전체 텍스트, 복사용)

```
안녕하세요, 취미 및 프로필 인증 기반 프리미엄 데이팅 앱 MVP 구축 프로젝트에 지원합니다.

본 프로젝트에 대한 상세 제안서(견적서, 공수계산서, PRD, 일정, 포트폴리오)를 별도 페이지로 준비하였습니다. 아래 링크에서 확인해 주시면 감사하겠습니다.
▶ 제안서 상세 페이지: https://proposal-router.claude-ai-b27.workers.dev/proposal-hobby-verified-dating-app-mvp/
▶ 위시켓 포트폴리오: https://www.wishket.com/partners/p/blueverse1/

---

<프로젝트 진행 제안>

■ 프로젝트 분석
- 취미·성향 인증 기반 신뢰 매칭 → 양방향 호감 표시 → 1:1 실시간 채팅으로 이어지는 프리미엄 데이팅 앱 MVP
- 소셜 로그인 + 휴대폰 본인 인증 + 관리자 인증 사진 심사 승인을 결합한 신뢰 게이트가 프리미엄 데이팅의 핵심 차별점
- 추천 피드(스와이프/리스트) + 나이·지역·취미 기본 필터 + 좋아요·매칭 + 매칭 성공 화면으로 이어지는 핵심 매칭 플로우
- Firebase/Supabase 기반 1:1 실시간 채팅 + FCM 푸시 알림으로 매칭·대화 즉시성 확보
- iOS/Android 동시 출시(Flutter 단일 코드베이스), 데이팅 카테고리 스토어 심사 정책 사전 점검
- 취미·성향 키워드와 매칭 로그를 정형화 적재하여 향후 추천 고도화 확장 대비

■ 작업 일정

[Phase 1] 기획 / 설계 — Day 1~12
- 킥오프, 서비스 기획·화면 설계, 매칭/키워드 정책 확정, 데이터 모델·아키텍처 설계
- 산출물: 화면 설계서, ERD/데이터 모델, 시스템 아키텍처 다이어그램

[Phase 2] 디자인 + 백엔드 착수 — Day 13~30
- Figma 디자인 시스템 → 앱/관리자 화면, Firebase/Supabase 구성
- 소셜 로그인·휴대폰 본인 인증·프로필 등록 모듈 우선 개발
- 산출물: Figma 원본, 인증·프로필 기능, BaaS 환경 가동

[Phase 3] 풀스택 개발 — Day 31~50
- 추천 피드·필터, 좋아요·매칭·매칭 성공 화면, 1:1 실시간 채팅, FCM 푸시, 관리자 백오피스 풀구현
- 산출물: 통합 베타 빌드 (TestFlight + Internal Testing)

[Phase 4] QA + 스토어 등록 + 출시 — Day 51~60
- 통합 QA 시나리오 테스트, App Store / Google Play 등록·심사 대응, 정식 출시
- 산출물: 앱 설치 파일·스토어 등록, 소스 코드 원본, 관리자 매뉴얼, 1개월 무상 하자보수 개시

■ 마일스톤 및 산출물
- M1 (Day 12): 기획·설계 완료 → 화면 설계서·ERD·아키텍처 승인
- M2 (Day 30): 디자인 완료 + 인증/프로필 데모 → Figma 전체 화면 승인, 로그인·본인인증·프로필 작동 확인
- M3 (Day 50): 통합 베타 빌드 → iOS/Android 설치, 추천·매칭·채팅·푸시 시나리오 통과
- M4 (Day 60): 정식 출시 → 스토어 정식 노출, 소스·관리자 매뉴얼 인계
- 최종 산출물: 화면 설계서, Figma 원본, 데이터 모델/ERD, 앱·관리자 소스 코드(소유권 클라이언트 귀속), 앱 설치 파일·스토어 등록, 관리자 매뉴얼

■ 미팅 시 협의 필요 사항
- 상세 기획 문서(제안요청서) 공유 및 화면/정책 디테일 확정
- 소셜 로그인 제공자 범위 (Google/Apple/Kakao)
- 휴대폰 본인 인증 기관 선정 (NICE / KCB 등) 및 계약 명의
- Firebase / Supabase 사용 범위 및 운영 계정 주체
- 관리자 백오피스 형태 (전용 웹 vs DB 직접 관리) 및 운영 권한 범위
- 데이팅 카테고리 Apple/Google 심사 정책 사전 점검 항목

---

<유사 프로젝트 진행 경험>

▶ Connectin — 디지털 명함 & 네트워킹 플랫폼 (2025.05~2025.08, 3개월)
- 프로젝트 유형: B2B 매칭·네트워킹 플랫폼
- 핵심 기능: 프로필 기반 매칭, BLE/GPS 근거리 탐색, Signal Protocol E2E 암호화 1:1 메시징, OCR 명함 스캔, 관리자 패널, 12 마이크로서비스
- 유사점: 프로필 기반 매칭 도메인 직접 경험(추천·좋아요·매칭·1:1 채팅 흐름 전이), Flutter 양대 마켓 출시, 관리자 패널 구축
- 기술 스택: Flutter, BLoC, Express, PostgreSQL, Firebase Auth/FCM, Docker

▶ Harmony Link — 통합 관리 플랫폼 (2025, 약 6개월)
- 프로젝트 유형: B2B SaaS 멀티플랫폼 (Flutter + NestJS)
- 핵심 기능: FCM 실시간 푸시 알림, Next.js 관리자 웹 패널 + RBAC 6개 역할, 카카오/네이버 소셜 로그인, Firebase Auth, 멀티테넌트 (133K+ LOC, 140+ API, 6개 플랫폼)
- 유사점: 본 프로젝트의 관리자 백오피스(인증 사진 심사·가입 승인)에 직접 대응되는 RBAC 관리자 웹 구축 경험, FCM 실시간 푸시 알림, Flutter 양대 마켓 + 소셜 로그인
- 기술 스택: Flutter 3.35, BLoC, NestJS 10, Next.js 13, MySQL, Firebase Auth/FCM, AWS

▶ Fortune App — Flutter B2C 운세 앱 (2024.07~2024.09, 3개월)
- 프로젝트 유형: B2C 라이프스타일 모바일 앱
- 핵심 기능: Google/Apple 소셜 로그인, 포인트·데일리 체크인 리워드, 결과 공유, Firebase Analytics/Remote Config, Clean Architecture(305 Dart 파일)
- 유사점: Flutter 단일 코드베이스로 3개월 내 기획~디자인~개발~스토어 출시 완수 패턴(60일 MVP 일정 근거), 소셜 로그인·Firebase 연동 동일
- 기술 스택: Flutter 3.22, BLoC/Cubit, Firebase, Node.js, Clean Architecture

---

<사용 기술과 툴>

▶ 개발 기술
- 모바일: Flutter 3.x, Dart, BLoC/Riverpod, Clean Architecture
- 백엔드/BaaS: Firebase (Auth, Firestore/RTDB, FCM, Storage), Supabase (Postgres/Realtime)
- 관리자 웹: Next.js, React, TypeScript, TailwindCSS
- 인증: 소셜 로그인 (Google/Apple), 휴대폰 본인 인증 (SMS)
- 실시간/알림: 실시간 채팅(RTDB/Realtime), FCM 푸시 + 딥링크

▶ 개발 도구 및 인프라
- 버전 관리: GitHub
- CI/CD: GitHub Actions (Flutter 빌드 자동화)
- 클라우드/BaaS: Firebase, Supabase
- 디자인: Figma (디자인 시스템 + 컴포넌트 라이브러리)

▶ 커뮤니케이션
- 일일 진행 공유: Slack 또는 카카오톡
- 주간 미팅: Zoom / Google Meet
- 문서 공유: Notion 또는 Google Docs
- 이슈 트래킹: GitHub Issues 또는 Linear
```

### 관련 포트폴리오 추천
1. **Connectin** — 프로필 기반 매칭·1:1 메시징 도메인 직접 경험 (Flutter 풀스택, 3개월 양대 마켓 출시, 관리자 패널)
2. **Harmony Link** — Next.js RBAC 관리자 백오피스 + FCM 실시간 푸시 + Flutter 소셜 로그인 (관리자 승인 시스템·알림 직접 대응)
3. **Fortune App** — Flutter B2C 3개월 풀패키지 양대 마켓 출시 + 소셜 로그인 (60일 일정 근거)
