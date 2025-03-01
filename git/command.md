# 명령어 정리

## `git init`
- 현재 디렉토리에 `.git` 폴더를 생성.

## `git clone` + url 
- 현재 디렉토리에 원격저장소 폴더를 복제.

## `git clone` + url + 설정이름
- 현재 디렉토리에 설정한 이름으로 원격저장소 폴더를 복제
    - 다른 사람의 파일을 clone한 경우, `.git`파일까지 가지고 옴
    - 따라서 따로 remote 추가할 필요 X
    - 작업 환경이 원파일을 작업하였던 환경값을 따라옴

## `git status`
- 현재 git의 상태를 확인
    - tracked, untracked 파일을 구분하여 표시

## `git add`
- working directory에서 변경된 파일을 staging area에 이동.

```
git add {file_name/directory_name}
git add . => 현재 나의 위치를 기준으로 모든 파일과 폴더
```

## `git commit` + -m + "인덱스메시지"
- staging area에 있는 변경사항을 커밋하여 스냅샷 생성

## `git log`
- 커밋의 히스토리를 조회
    - option
        - `--oneline`
        - `--graph` 협업 타임라인 확인에 유용

## `git remote`

### **원격저장소 관리 명령어**
#### - git 과 로컬을 연결해주는 선(git에서 부여받은 url) (git과 파일, 폴더에는 영향X)

- 원격저장소 추가

```
git remote add {remote_name} {remote_url}
```
- 원격저장소 확인
```
git remote -v
```
- 원격저장소 삭제
```
git remote remove
```

## `wq`
- 입력 후 나가기

## `q`
- 나가기

## `git push origin master`
- github에 수정, 스냅샷 찍은 최종파일을 올리다.

## `git pull origin master`
- github으로부터 최신 파일을 불러오다.