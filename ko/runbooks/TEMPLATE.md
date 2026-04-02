---
title: 템플릿
---

<div id="agent-prompt-task-title">
  # 에이전트 프롬프트: [Task title]
</div>

<div id="requirements">
  ## 요구 사항
</div>

이 작업을 시작하기 전에 필요한 접근 권한 또는 선행 조건을 모두 나열하십시오:

- [ ] 필수 시스템 접근 권한(예: W&B 직원 접근 권한)
- [ ] 필수 권한(예: 저장소 쓰기 권한)
- [ ] 필수 도구 또는 종속성

<div id="agent-prerequisites">
  ## 에이전트 사전 요구사항
</div>

시작하기 전에 사용자로부터 수집해야 할 정보:

1. **[Required info 1]** - 필요한 이유
2. **[Required info 2]** - 필요한 이유
3. **[Optional info]** - 언제/왜 필요할 수 있는지

<div id="task-overview">
  ## 작업 개요
</div>

이 런북이 수행하는 작업과 사용 시점을 간단히 설명합니다.

> **참고**: 사용자가 사전에 알아야 할 중요한 배경 정보나 제한 사항을 여기에 명시하십시오.

<div id="context-and-constraints">
  ## 맥락 및 제약 조건
</div>

<div id="systemtool-limitations">
  ### 시스템/도구 제한 사항
</div>

- 제한 사항 1과 작업에 미치는 영향
- 제한 사항 2와 (있는 경우) 우회 방법

<div id="important-context">
  ### 중요한 참고 사항
</div>

- 핵심 배경 정보
- 주의해야 할 일반적인 함정 또는 엣지 케이스
- 보안 관련 유의 사항

<div id="step-by-step-process">
  ## 단계별 절차
</div>

<div id="1-first-major-step">
  ### 1. [첫 번째 주요 단계]
</div>

이 단계에서 어떤 작업이 수행되는지에 대한 설명입니다.

```bash
# 예시 명령어
command --with-flags
```

**예상 결과**: 이 단계를 수행한 뒤에 일어나야 하는 일.


<div id="2-second-major-step">
  ### 2. [두 번째 주요 단계]
</div>

설명과 의사결정 지점을 기재합니다.

**에이전트 메모**: AI 에이전트를 위한 특별 지침 예시는 다음과 같습니다.

- 사용자에게 추가 설명을 요청해야 하는 시점
- 권한이 부족할 때 사용할 폴백(fallback) 절차
- 자주 발생하는 변형 사례를 처리하는 방법

<div id="3-continue-with-remaining-steps">
  ### 3. [나머지 단계 계속하기...]
</div>

<div id="verification-and-testing">
  ## 검증 및 테스트
</div>

예상 결과:

- ✓ 성공 지표 1
- ✓ 성공 지표 2
- ✗ 일반적인 실패 징후와 그 의미

<div id="how-to-verify-success">
  ### 성공 여부 확인 방법
</div>

1. 다음을 확인합니다:
2. 다음을 검증합니다:
3. 다음과 같이 테스트합니다:

<div id="common-issues-and-solutions">
  ## 자주 발생하는 문제 및 해결 방법
</div>

<div id="issue-common-problem-1">
  ### 문제: [Common problem 1]
</div>

- **증상**: 문제가 나타나는 양상
- **원인**: 발생 원인
- **해결 방법**: 단계별 해결 방법

<div id="issue-common-problem-2">
  ### 문제: [Common problem 2]
</div>

- **증상**: 
- **원인**: 
- **해결 방법**: 

<div id="cleanup-instructions">
  ## 정리 지침
</div>

작업을 완료한 후 다음을 수행하세요:

1. 임시 파일/브랜치를 모두 삭제합니다.
2. 수정된 설정을 모두 원래대로 되돌립니다.
3. 수행한 영구적인 변경 사항을 모두 문서화합니다.

```bash
# 정리 명령어 예시
git branch -D temp-branch-name
rm -f temporary-files
```


<div id="checklist">
  ## 체크리스트
</div>

전체 프로세스에 대한 요약 체크리스트:

- [ ] 모든 요구 사항을 충족했는지 확인합니다.
- [ ] 사용자로부터 필요한 정보를 모두 수집했는지 확인합니다.
- [ ] 1단계를 완료했는지 확인합니다: [간단한 설명].
- [ ] 2단계를 완료했는지 확인합니다: [간단한 설명].
- [ ] 결과를 검증했는지 확인합니다.
- [ ] 임시 리소스를 정리했는지 확인합니다.
- [ ] 영구적인 변경 사항을 문서화했는지 확인합니다.

<div id="notes">
  ## 참고 사항
</div>

- 추가적인 팁 또는 맥락.
- 관련 문서 링크.
- 대체 접근 방식을 언제 사용할지.