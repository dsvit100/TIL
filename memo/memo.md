## 250211 화

### 1. git book
- git 파일 내 basic.md, command.md 참고

### 2. github page (PR페이지 만들기 - 도메인은 계정 당 하나만 가능)
> 참고사이트: [star bootstrap](https://startbootstrap.com/themes)
- PR페이지 작업할 폴더 생성
- 원하는 템플릿을 다운로드(대부분 zip파일) 후 압축풀기
- 압축 푼 파일을 PR작업 폴더로 끌어서 이동(폴더째 옮기기X)
- git에 새 저장소(repository) 생성
- git과 로컬을 연결하기 위해 원격저장소 만들기 `git remote add` + url
    - 수정하지 않은 채로 바로 push 불가!
    - 다운로드 받은 파일 그대로(수정없이) 올리는 경우 add - commit - push 해 줘야만 git에 원격저장소가 만들어짐


### 3. end-to-end (끝말잇기)
- 파일 공유하기 (A - B)
    - A : git 접속 - 공유할 파일 내에서 setting - collaborators - people
    git아이디 입력 후 초대
    - B : 메일 확인 후 수락 - git으로 관리할 폴더 내 빈공간에 우클릭 open git bash here
        - ***왜?***
        공유 파일(폴더)를 작업하려면 ex)end-to-end 파일이 있어야 하는데
        끌어올 파일이 없으므로 open git bash here 통해서 터미널 열어준 다음
        clone 작업해야함.


