# Kustomize 를 사용한 배포자동화

1. Front, Backend Repo에 push
2. 각 Repo 의 Github Action 동작, Build
3. ECR로 이미지 push. push 한 이미지의 tag 기억
4. 기억한 Tag를 현재의 Master Branch의 overlays/prd 로 update
5. 