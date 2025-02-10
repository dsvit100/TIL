# 리눅스 기본명령어

## 0. 명령어의 기본형식
```
command [options] [arguments]
```

- command : 실행할 명령어, 프로그램
- options : 명령어의 옵션
- arguments : 명령어에 전달할 인자(값)

## 1. 파일 및 디렉토리 관리

### ls (list)
- 현재 내 위치에 열 수 있는 모든 디렉토리 내용 목록을 보여줍니다.
- options :
    - `-l` : 파일의 상세 정보 표시
    - `-a` : 숨김 파일 표시
    - . 은 현재폴더 / ..은 상위폴더

    ### cd (change directory)
        - 현재 작업 디렉토리를 변경합니다. (맥에서는 pwd - print work)
        - `cd {target-directory}`
            - target-directory는 자동완성 기능을 활용(TAB)
        - cd + TAB(공통앞자리까지 나와줌)
        - 만약 폴더명을 기억하지 못 한다면 위의 탭 이후 탭 두번
        - ~ = 사용자의 즐겨찾기 (데스크톱의 윗단계)

    ### pwd (print working directory)
    - 현재 작업 중인 디렉토리의 전체 경로를 출력.

    ### mkdir (make directory)
    - 새로운 디렉토리를 생성.
    - `mkdir {directory-name}`

    ### touch
    - 새로운 파일을 생성.
    - `touch {file-name}`

    ### rm (remove)
    - 파일이나 폴더를 삭제.
    - options
        - `-r` : 디렉토리와 그 내용을 재귀적으로 삭제
        - 폴더 안에 또 폴더와 파일이 있을 수 있으므로 폴더는 rm만으로는 삭제가 안됨
    
    ### cat (concatenate)
    - 파일의 내용을 출력.
    
