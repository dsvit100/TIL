# intro
### shortcut
- ctrl + enter : 현재 셀 실행
- shift + enter : 현재 셀 실행 & 아래로 이동
- alt + enter : 현재 셀 실행 & 아래에 새로운 셀 추가

# 1. 변수
- number, boolean, string
```python
var_name(변수이름) = value(값)
# a = 1
# a = 1이 아니라
# a라는 상자에 1을 넣는다는 개념
```
- 변수 이름은 어떤 이름이든 사용 가능
    - 한글 사용 가능하지만 지양하기
- 영어, 숫자, _ 를 이용해서 선언
- 파이썬의 기능을 가진 이름들(키워드)는 사용X
```python
- 파이썬 키워드 확인하기
import keyworld
keyword.kwlist
```

## 1.1 number
- int: 정수
- float: 실수
    - 컴퓨터는 물리적으로 소수 저장 x = 부동소수점
    - (두루뭉술하게 표시하다보니 float라고 표현)
- complex: 복소수

## 1.2 boolean(불리언)
- True / False

## 1.3 문자열 ('', "")
```python
print('hello my name is "hyojin"')
# ''안의 ""는 충돌 없이 출력
# ''는 문자열을 작성하는 기호지만
# 값 내 ''까지 출력되길 원하면 \'\'으로 표기
print('hello my name is \'hojin\'')
# 문자열('')에서는 줄바꿈이 들어가지 않는 것이 일반적
# (''' ''')로 묶는 경우 줄바꿈 포함하여 출력(print) 가능
a = '''
hello
world
hi
'''
# 출력값:
hello
world
hi
```

### string interpolation (문자열 안에 변수 삽입 방법)
- %-fomatting
```python
age = 10
print('홍길동은 %s살입니다.' % age)
# %s는 문자열, %d는 정수를 의미
```
- st.format()
```python
print('홍길동은 {}살입니다.'.format(age))
# %-formatting보다 가독성 좋음
```
- f-string
```python
print(f'홍길동은 {age}살입니다.')
# f를 문자열 앞에 붙이고 {}안에 변수를 배치
```

# 2. 연산자
## 2.1 산술연산자
```python
+, -, *, /
** 제곱, // 몫만 출력, % 나머지만 출력
divmod(a, b) 몫과 나머지 모두 출력
```
## 2.2 논리연산자
- and : 양쪽 모두를 만족해야 True, 하나라도 만족하지 않으면 False
- or : 한쪽만 만족해도 True, 둘다 만족하지 않으면 False
- not : 상태를 부정
```python
a = true
print(not a)
# 값은 False
```
## 2.4 복합연산자 >> 질문해보자
print(a %= b) 값이 안나옴..ㅠ

## 2.5 기타연산자
- 글자끼리는 concatenation(연결), 숫자끼리는 연산이 됨.
- 먼저 제시된 값에 따라 연결 / 연산으로 인식함
```python
num = input()
if num % 2 == 1:
    print('odd')
else:
    print('even')
# 이 경우 오류: %가 연산기호로 적용되지 않았기 때문
# num을 int() 이용하여 숫자로 변경해줘야함