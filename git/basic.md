# GIT 기본 개념

## 분산버전 관리 시스템
- 클라이언트와 서버 모두가 똑같은 데이터를 유지하여 버전을 관리하는 시스템

## 파일의 세가지 상태

![areas](../assets/areas.png)

- 영역
    - working directory : 작성하고 있는 코드, 파일
    - staging aria : add 명령어로 무대 위로 올라간 파일들
    - .git directory(repository) : commit 명령어로 찍힌 스냅샷들을 저장

### CLI (commend line interface)
- 컴퓨터와 소통하기 위한 수단

## 파일의 라이프 사이클
![lifecycle](https://git-scm.com/book/ko/v2/images/lifecycle.png)

- Tracked(관리대상임)와 Untracked(관리대상이 아님)
    - Unmodified(수정하지 않음),modified(수정함), staged(커밋으로 저장소에 기록함)
    - untracked : 워킹 디렉토리에 있는 파일 중 스냅샷에도 staging Area에도 포함되지 않은 파일이다.
    

- http://gitignore.io/ : git에서 무시하고 싶은 파일 설정 사이트
    - ![git_ignore_files](../assets/git_ignore_files.png)