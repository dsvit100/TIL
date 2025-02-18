# 함수(function)
## 함수의 선언과 호출
- 선언
```python
def func_name(paramiter1, paramiter2, ...):
    code1
    code2
    ...
    return value
# 함수 선언 시 값을 지정해버리면 이후에 함수 호출 시 작동 X
# 함수 작성할 때 쓴 값이 적용되기 때문에
```
- 호출
`func_name(paramiter1, paramiter2, ...)`
- 새 함수명은 파이썬 설치 시 미리 만들어져있는 함수명과 중복될 수 없음
    - `dir(__builtins__)`
    - 중복될 경우 기존 함수에 덮어쓰기 됨
    - 덮어쓰기 되면 커널 재실행하기

## 함수의 return
- 함수가 return을 만나면 해당값을 반환하고 함수를 종료
- 만약 return이 없는 경우 None을 자동으로 반환
- return은 오직 하나의 객체만 반환