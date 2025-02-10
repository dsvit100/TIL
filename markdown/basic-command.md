# 0. 왜 markdown을 사용하는가?
- 어떤 환경에서든 일관된 양식 작성을 위해

# 0-1 노션 / 옵시디언
- 노션
    - 클라우드 서비스, 서버가 죽었을 때 접근 X
- 옵시디언
    - 로컬(기기)에 저장됨

# 1. 제목
- 1~6개의 # 기호를 사용하여 제목 수준 지정 (ex. #, ##, ###)

## 예시 중제목

# 2. 텍스트 스타일
- 굵게: **단어**
- 기울게: *단어*
- 취소: ~~단어~~
- 굵고 기울게: ***단어***


# 3. 텍스트 인용
> 인용구문
> 여러줄도 가능합니다.

# 4. 코드 인용

- 인라인 코드 인용 => `code` 해당 하이라이트는 코드 인용에 사용이 일반적이다!
- 코드블럭
```python
def hello(): 
    print("hello!")
```

```javascript
console.log("hello")
```

# 5. 링크
- [구글](https://google.com)

# 6. 이미지
- ![귀여운키링](https://image.artbox.co.kr/upload/C00001/goods/800_800/249/240315005125249.jpg?s=/goods/org/249/240315005125249.jpg)
- ![귀여운키링](../assets/keyring.jpg)
    - 하위 이미지는 로컬에 저장된 파일을 불러온 것으로 상대적임
이미지를 한글명으로 기입하면 적용X
- 이미지 입력 시 대괄호에 텍스트 입력하는 이유:
이미지 코드에 오류가 났을 때 대체할 수 있는 이미지(엑박 등)가 필요하기 때문

# 7. 목록

## 순서있는목록
1. 첫번째
2. 두번째
3. 세번째
## 순서없는목록
- 첫번째
    - 1-1
    - 1-2
- 두번째
- 세번째
**위의 7가지는 모든 markdown에 적용되는 문법**

[출처](https://docs.github.com/ko/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings)

- [x] 할일목록