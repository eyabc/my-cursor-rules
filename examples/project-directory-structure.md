# 📁 프로젝트 디렉터리 구조
```
TravelAI/
├── backend/                     # Next.js 백엔드 서버
│   ├── .next/                   # Next.js 빌드 결과물 및 캐시
│   ├── prisma/                  # 데이터베이스 스키마 및 마이그레이션
│   ├── public/                  # 정적 파일 (이미지, 아이콘 등)
│   └── src/                     # 백엔드 소스 코드
├── TravelAIApp/                 # Flutter 모바일 애플리케이션
│   ├── android/                 # Android 플랫폼 설정
│   ├── ios/                     # iOS 플랫폼 설정
│   ├── lib/                     # Flutter 앱 소스 코드
│   ├── test/                    # 유닛 테스트 파일
│   └── build/                   # 앱 빌드 결과물
├── src/                         # 공통 프론트엔드 코드
│   ├── api/                     # API 호출 관련 코드
│   ├── store/                   # 상태 관리 (Redux/Context)
│   └── types/                   # TypeScript 타입 정의
├── cursor-memory-bank/          # AI 개발 워크플로우 메모리 뱅크
│   ├── archive/                 # 완료된 작업 아카이브
│   ├── creative/                # 창작 단계 문서
│   ├── reflection/              # 작업 회고 문서
│   ├── assets/                  # 공유 리소스 및 템플릿
│   └── custom_modes/            # 커스텀 AI 모드 설정
├── .roo/                        # Roo AI 시스템 규칙 및 설정
│   ├── rules/                   # 기본 개발 규칙
│   ├── rules-architect/         # 아키텍처 모드 규칙
│   ├── rules-ask/               # 질문 모드 규칙
│   ├── rules-boomerang/         # 부메랑 모드 규칙
│   ├── rules-code/              # 코드 모드 규칙
│   ├── rules-debug/             # 디버그 모드 규칙
│   └── rules-test/              # 테스트 모드 규칙
├── tasks/                       # 작업 관리 및 진행 상황
├── scripts/                     # 유틸리티 스크립트 및 문서
└── .expo/                       # Expo 개발 환경 설정
```

## 📖 디렉터리 설명

### 🖥️ Backend (`/backend`)
Next.js 기반의 백엔드 API 서버입니다.
- **prisma/**: PostgreSQL 데이터베이스 스키마, 마이그레이션 파일
- **src/**: API 라우트, 비즈니스 로직, 유틸리티 함수
- **public/**: 정적 파일 제공 (이미지, 파비콘 등)
- **.next/**: Next.js 빌드 캐시 및 최적화된 결과물

### 📱 Mobile App (`/TravelAIApp`)
Flutter로 개발된 크로스플랫폼 모바일 애플리케이션입니다.
- **lib/**: Dart/Flutter 소스 코드 (위젯, 모델, 서비스 등)
- **android/**: Android 플랫폼별 설정 및 네이티브 코드
- **ios/**: iOS 플랫폼별 설정 및 네이티브 코드
- **test/**: 유닛 테스트 및 위젯 테스트

### 🌐 Frontend Common (`/src`)
프론트엔드 공통 코드 및 타입 정의입니다.
- **api/**: REST API 호출 함수들
- **store/**: 전역 상태 관리 (Redux Toolkit/Context API)
- **types/**: 공통 TypeScript 인터페이스 및 타입

### 🧠 AI Development System (`/cursor-memory-bank`)
AI 기반 개발 워크플로우를 위한 메모리 뱅크 시스템입니다.
- **archive/**: 완료된 작업의 상세 기록
- **creative/**: 기능 설계 및 창작 단계 문서
- **reflection/**: 작업 완료 후 회고 및 학습 내용
- **assets/**: 템플릿, 가이드라인, 공유 리소스
- **custom_modes/**: AI 어시스턴트 커스텀 모드 정의

### ⚙️ AI Rules System (`/.roo`)
Roo AI 시스템의 모드별 규칙 및 행동 지침입니다.
- **rules/**: 기본 개발 및 코딩 규칙
- **rules-architect/**: 시스템 아키텍처 설계 규칙
- **rules-ask/**: 질문 및 분석 모드 규칙
- **rules-boomerang/**: 작업 오케스트레이션 규칙
- **rules-code/**: 코드 구현 모드 규칙
- **rules-debug/**: 디버깅 및 문제 해결 규칙
- **rules-test/**: 테스트 작성 및 실행 규칙

### 📋 Task Management (`/tasks`)
프로젝트 작업 계획 및 진행 상황 추적을 위한 Task Master 시스템입니다.
- 개별 작업 파일들 (task_001.txt ~ task_013.txt)
- **tasks.json**: 전체 작업 구조 및 의존성 정의

### 📜 Scripts & Documentation (`/scripts`)
프로젝트 문서 및 유틸리티 스크립트입니다.
- **prd.txt**: 제품 요구사항 문서 (Product Requirements Document)
- **task-complexity-report.json**: 작업 복잡도 분석 결과
- **example_prd.txt**: PRD 작성 예시 템플릿

### 📲 Expo Configuration (`/.expo`)
React Native/Expo 개발 환경 설정 및 캐시 파일들입니다.
