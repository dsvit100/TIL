# 250210 월

## 1. 작업에 필요한 환경 만들기
- git : 모든 체크 사항 건드리지 않고 인스톨
- vscode(코드를 입력하는 메모장) : 체크박스 2개 확인 후 인스톨
- python(언어) : add to pass 필수 체크 후 인스톨
- 구글드라이브
- slack

## 2. mark down
> 워드, 한글 등의 파일에 따라 양식이 일관되게 적용되지 않는 점을 고려하여
어떠한 사양에서든 일관된 양식 작성을 위해 markdown의 양식을 사용한다.
- 노션 / 옵시디언
    - 노션 : 클라우드 서비스, 서버가 죽었을 때 접근 불가
    - 옵시디언 : 로컬(기기)에 저장됨

## 3. GIT
> 사용자의 수정 내역을 트래킹 할 수 있게 함
- 수정1, 수정2... 같이 넘버링하고 재저장 할 필요 없이 최종 버전까지 쭉 작성됨. 
단, 수정된 부분은 색상 변경으로 표시되고 수정 제목도 라벨링 된다.




# 250211 화


## 1. git book
- git 파일 내 basic.md, command.md 참고


## 2. github page (PR페이지 만들기 - 도메인은 계정 당 하나만 가능)
> 참고사이트: [star bootstrap](https://startbootstrap.com/themes)
- PR페이지 작업할 폴더 생성
- 원하는 템플릿을 다운로드(대부분 zip파일) 후 압축풀기
- 압축 푼 파일을 PR작업 폴더로 끌어서 이동(폴더째 옮기기X)
- git에 새 저장소(repository) 생성
- git과 로컬을 연결하기 위해 원격저장소 만들기 `git remote add` + url
    - 수정하지 않은 채로 바로 push 불가!
    - 다운로드 받은 파일 그대로(수정없이) 올리는 경우 add - commit - push 해 줘야만 git에 원격저장소가 만들어짐


## 3. end-to-end (끝말잇기)
- 파일 공유하기 (A - B)
    - A : git 접속 - 공유할 파일 내에서 setting - collaborators - people
    git아이디 입력 후 초대
    - B : 메일 확인 후 수락 - git으로 관리할 폴더 내 빈공간에 우클릭 open git bash here
        - ***왜?***
        공유 파일(폴더)를 작업하려면 ex)end-to-end 파일이 있어야 하는데
        끌어올 파일이 없으므로 open git bash here 통해서 터미널 열어준 다음
        clone 작업해야함.

- 작업하다 충돌된 경우
    - 가장 최근 파일로 pull
    - 모두 지우고 새로 쓰기 / 선택하기
    - current - 내것 / incoming - 외부의 것 / both - 둘 다 합치기 