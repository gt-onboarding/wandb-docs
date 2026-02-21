---
title: "라이선스 고지"
---

<div id="license-notice-for-reference-documentation-generation">
  # 레퍼런스 문서 생성을 위한 라이선스 고지
</div>

<div id="overview">
  ## 개요
</div>

이 디렉터리의 스크립트는 개발/CI 프로세스 중 레퍼런스 문서를 생성하는 데에만 사용됩니다. 이 스크립트는 Weave 라이브러리와 함께 배포되지 않으며, 어떤 프로덕션 코드에도 포함되지 않습니다.

<div id="dependencies-and-their-licenses">
  ## 종속성 및 해당 라이선스
</div>

<div id="direct-dependencies">
  ### 직접 의존성
</div>

- **requests** (Apache-2.0): HTTP 요청을 보내는 데 사용
- **lazydocs** (MIT): W&B에서 유지 관리하는 문서 생성기

<div id="transitive-dependencies-via-lazydocs">
  ### 전이적 의존성 (lazydocs를 통해)
</div>

- **setuptools** (MIT, 일부 LGPL-3.0 컴포넌트 벤더링): 빌드 시스템
- 기타 여러 혼합 라이선스 의존성

<div id="important-notes">
  ## 중요 사항
</div>

1. **개발 전용**: 이 종속성들은 CI/GitHub Actions에서 문서 생성 중에만 일시적으로 설치됩니다. 배포되는 Weave 패키지에는 절대 포함되지 않습니다.

2. **비배포 대상**: 생성된 문서는 실행 가능한 코드나 종속성 없이 MDX/Markdown 파일로만 구성됩니다.

3. **격리된 실행**: GitHub Actions는 사용 후 삭제되는 격리된 가상 환경에서 이러한 스크립트를 실행합니다.

4. **라이선스 준수**: 이 도구들은 Weave와 함께 배포되지 않으므로, `setuptools`의 번들 종속성에 포함된 LGPL-3.0 구성 요소들은 Weave 사용자에게 라이선스 의무를 발생시키지 않습니다.

<div id="for-organizations-with-strict-license-policies">
  ## 엄격한 라이선스 정책을 가진 조직의 경우
</div>

조직에서 개발 도구에 어떠한 LGPL 코드 사용도 금지하는 정책이 있는 경우 다음을 수행하십시오:

1. GitHub Action을 사용해 클라우드에서 문서를 생성합니다(권장)
2. lazydocs 사용을 피하는 최소한의 Python 기반 생성기를 사용합니다
3. Docker 컨테이너에서 문서를 생성합니다
4. 개발 전용 도구에 대해 예외를 요청합니다

<div id="socket-security">
  ## 소켓 보안
</div>

리포지토리 루트 디렉터리의 `.socketignore` 파일은 다음 스크립트들이 프로덕션 코드가 아닌 개발 도구이므로 보안 스캔 대상에서 제외합니다.

<div id="known-socket-security-warnings">
  ### 알려진 소켓 보안 경고
</div>

- **wheel 내 네이티브 코드**: `wheel` 패키지에는 네이티브 코드가 포함되어 있는데, 이는 Python 패키징 도구에서는 일반적인 구성입니다
- **라이선스 위반**: 일부 전이적 의존성에 LGPL 또는 기타 라이선스가 포함되어 있어 정책 경고를 트리거할 수 있습니다

이러한 경고는 다음과 같은 이유로 허용됩니다:

1. 해당 도구들은 문서 생성 시에만 사용됩니다
2. 격리된 CI 환경에서만 실행됩니다
3. Weave와 함께 배포되지 않습니다
4. 생성된 문서에는 실행 가능한 코드가 포함되어 있지 않습니다