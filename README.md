# aws9d Helm Chart

## 설명
이 Helm Chart는 `default`, `shop`, `blog`, `news` 웹 서비스를 배포하며,
자동 PVC 생성, Ingress 연동, KEDA 오토스케일링이 포함되어 있습니다.

## 사전 조건
- Metallb가 설치되어 있어야 합니다
- Ingress Nginx Controller가 배포되어 있어야 합니다
- hub.aws9.pri에 접속 가능한 Harbor가 있어야 합니다

## 설치 방법

```bash
helm repo add aws9repo https://jjeonge38.github.io/k8s_mini_helm
helm install aws9test aws9repo/aws9-web