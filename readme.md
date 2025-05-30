# My Rules Trigger 규칙 문서

## 개요
이 문서는 `.cursor/rules/my_rules` 디렉토리 내의 모든 .mdc 파일들의 trigger 규칙을 정리하고 문서화합니다. 각 규칙의 목적, 적용 범위, 동작 방식을 상세히 설명합니다.

## Trigger 패턴
- 기본 패턴: `.cursor/rules/my_rules/**/*.mdc`
- 감지 범위: my_rules 디렉토리 및 모든 하위 디렉토리의 .mdc 파일들

## 현재 등록된 Rules

### 1. 프로젝트 디렉토리 구조 Rule
- **파일**: `init-directory-description-rules.mdc`
- **설명**: 프로젝트 루트로부터 depth 2까지의 디렉터리 및 파일 구조를 트리 형태로 문서화
- **Globs**: `["@.cursor/docs/project-directory-structure.md"]`
- **관련 문서**: `["@rules/my_rules/example/project-directory-structure.mdc"]`
- **주요 기능**:
  - 디렉토리 구조의 자동 문서화
  - 신규 팀원 온보딩 지원
  - 자동화 도구의 프로젝트 구조 파악 지원

### 2. My Rules Trigger Rule
- **파일**: `my-rules.mdc`
- **설명**: my_rules 디렉토리의 .mdc 파일 변경 감지 및 trigger 설정
- **Globs**: `[".cursor/rules/my_rules/**/*.mdc"]`
- **주요 기능**:
  - 규칙 파일 변경 자동 감지
  - 규칙 변경 시 즉시 적용
  - 규칙 파일 관리 자동화

## Trigger 동작 방식

### 자동 감지 이벤트
1. 새로운 .mdc 파일 추가
2. 기존 .mdc 파일 내용 수정
3. .mdc 파일 삭제

### 처리 프로세스
1. 파일 변경 감지
2. 규칙 유효성 검증
3. 규칙 적용 및 활성화
4. 변경 사항 로깅

## 규칙 적용 우선순위
1. 직접 지정된 파일 규칙
2. 디렉토리 범위 규칙
3. 전역 규칙

## 유지보수 가이드라인

### 규칙 추가 시
- 명확한 설명과 목적 정의
- 적절한 glob 패턴 설정
- 관련 문서 참조 추가
- 테스트 및 검증

### 규칙 수정 시
- 변경 사항 문서화
- 영향 범위 분석
- 하위 호환성 고려
- 테스트 케이스 업데이트

### 규칙 삭제 시
- 삭제 사유 문서화
- 의존성 검사
- 대체 규칙 제시
- 영향 받는 시스템 업데이트

## 주의사항
- 규칙 변경 시 프로젝트 전체에 미치는 영향 고려
- 중복 규칙 방지
- 명확한 네이밍 컨벤션 준수
- 정기적인 규칙 검토 및 업데이트 