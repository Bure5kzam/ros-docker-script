# 개요

ros2 어플리케이션을 도커에서 실행하는 프로젝트.

현재는 devcontainer로만 실행되도록 구성되어있음. (추후 compose로 여러개 실행할 수 있도록 구현 예정)

vscode에서 워크스페이스로 열면 관련 도커 컨테이너가 실행됨.

# 사전 세팅

1. `/src`에 실행할 ros2 패키지들을 배치한다.
2. `devcontainer.json` 에서 `username` 값을 현재 시스템의 사용자명과 일치시킨다. (파일 생성 권한 문제) 


---

사용하는 두 가지 방법이 잇음.

# devcontainer

vscode로 워크스페이스를 열면 컨테이너가 자동 실행되도록 되어있음.

컨테이너 내에서 의존성 설치, 빌드하는 용도로 사용하기위해 구성했다.

## 실행방법

1. `View->Command Palette...` 또는 `Ctrl+Shift+P` 로 커맨드 팔레트를 열어서 `Dev Containers: Reopen in Container and execute` 를 실행.

<!-- Use View->Command Palette... or Ctrl+Shift+P to open the command palette. Search for the command Dev Containers: Reopen in Container and execute it. This will build your development docker container for your. It will take a while - sit back or go for a coffee. -->


## 주의사항

- `devcontainer.json` 에서 `username`을 현재 시스템의 사용자명과 일치시켜야함. (파일 생성 권한 문제) 


# docker compose

docker compose로 필요한 서비스를 실행할 수 있음.

컨테이너 내에서 ros2 어플리케이션을 실행하는 용도로 사용하기위해 구성했다.