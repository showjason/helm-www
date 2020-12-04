---
title: "Helm Test"
---

## helm test

릴리스에 대하여 테스트를 수행한다.

### 개요


test 명령어는 릴리스에 대한 테스트를 실행한다.

이 명령어가 받는 인수는 배포된 릴리스의 이름이다.
실행할 테스트는 설치된 차트에 정의되어 있다.

```
helm test [RELEASE] [flags]
```

### 옵션

```
  -h, --help               helm test 에 대한 도움말
      --logs               테스트 파드에서 로그를 덤프 (모든 테스트가 완료된 후 정리 전에 실행)
      --timeout duration   개별 쿠버네티스 작업(예: 훅에 대한 작업)을 기다리는 시간 제한 (기본값 5m0s)
```

### 부모 명령어에서 상속된 옵션들

```
      --debug                       장황한(verbose) 출력 활성화
      --kube-apiserver string       쿠버네티스 API 서버의 주소 및 포트
      --kube-as-group stringArray   작업에 관해 제시할 그룹. 플래그를 여러 번 사용하여 여러 그룹 지정 가능
      --kube-as-user string         작업에 관해 제시할 사용자명
      --kube-context string         사용할 kubeconfig 컨텍스트 이름
      --kube-token string           인증에 사용될 베어러(bearer) 토큰
      --kubeconfig string           kubeconfig 파일 경로
  -n, --namespace string            이 요청에 대한 네임스페이스 스코프
      --registry-config string      레지스트리 구성 파일에 대한 경로 (기본값 "~/.config/helm/registry.json")
      --repository-cache string     캐시된 저장소 색인이 포함된 파일의 경로 (기본값 "~/.cache/helm/repository")
      --repository-config string    저장소 이름 및 URL 을 포함하는 파일 경로 (기본값 "~/.config/helm/repositories.yaml")
```

### SEE ALSO

* [helm](../helm)	 - 쿠버네티스에 대한 헬름 패키지 매니저.

###### Auto generated by spf13/cobra on 29-Oct-2020