# 개요

ros2 어플리케이션을 도커에서 실행하는 프로젝트.

현재는 devcontainer로만 실행되도록 구성되어있음. (추후 compose로 여러개 실행할 수 있도록 구현 예정)

vscode에서 워크스페이스로 열면 관련 도커 컨테이너가 실행됨.

# 사전 세팅

1. `/src`에 실행할 패키지들을 구성
2. `devcontainer.json` 에서 `username`을 현재 시스템의 사용자명과 일치시켜야함. (파일 생성 권한 문제) 


# 실행방법

`/src` 에 패키지 소스코드를 넣고 컨테이너를 실행해야함.

1. `View->Command Palette...` 또는 `Ctrl+Shift+P` 로 커맨드 팔레트트를 열어서 `Dev Containers: Reopen in Container and execute` 를 실행.

<!-- Use View->Command Palette... or Ctrl+Shift+P to open the command palette. Search for the command Dev Containers: Reopen in Container and execute it. This will build your development docker container for your. It will take a while - sit back or go for a coffee. -->


# 주의사항

- `devcontainer.json` 에서 `username`을 현재 시스템의 사용자명과 일치시켜야함. (파일 생성 권한 문제) 