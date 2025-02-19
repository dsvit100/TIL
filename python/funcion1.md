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

## 함수의 인수
### 위치인수
- 기본적으로 함수는 위치를 기준으로 인수 판단
```python
def cylinder(r, h):
    return 3.14 * 4 ** 2 * h
```
- 위의 식에서 r은 반지름, h는 높이값
- 반지름과 높이값을 바꿔 입력하면 원하는 값이 도출 X (위치값 확인하고 넣기)

### 기본값
```python
def func_name(p1=v1):
    code1
    return value

(예)
def greeting(name='익명'):
    return f'{name}님 반갑습니다.'
이 경우, `greeting()`으로 빈 값을 출력해도 '익명님 반갑습니다'가 출력됨
위의 형태로 작성하는 경우, ()는 필수값이 아님
임시('익명')로라도 넣어서 출력해줌
```

## 키워드인수
- 함수를 호출(실행)할 때 내가 원하는 위치에 직접적으로 값을 전달
```python
def greeting(age, name='익명'):
    retunr f'{name}님은 {age}살입니다.'
age는 필수 입력, name은 적지 않을 경우 '익명'으로 출력됨

- `greeting()`은 동작 X
(필수값 입력하지 않았기 때문에)
- `greeting(10)`은 동작 O
('익명'님은 10살입니다.)
- `greeting('길동')`은 동작 O
('익명'님은 '길동'살입니다.)
```

## 가변인자 리스트
- 사용자가 몇 개의 데이터를 입력할지 모르는 경우 사용
- 각 데이터를 위해 변수명을 계속 지정할 수 없으므로
- 하나의 묶음(tuple)으로 인식, 출력하게끔 함

```python
def func_name(*parms):  # *표가 된 것이 가변인자
# 몇 개의 인자가 들어오더라도 하나로 묶어줘.
    code
    ...
    return value
```

## 정의되지 않은 키워드 인자 처리하기 # n_help
```python
def func_name(**keyword arguments):
    return value
```
```python
def my_func(params1, params2='temp', *numbers, **kwargs):
    return 0
```
```python
# my_func() => params1 부족
my_func(123)
# => params1 = 123, params2 = 'temp'
my_func(123, 234)
# => params1 = 123, params2 = 234
my_func(123, 234, 345, 456)
# params1 = 123, params 2 = 234, params3 = numbers(345부터 모두)
my_func(123, 234, 345, 456, a=1, b=2, c=3)
# kwargs = {a: 1, b: 2, c: 3}
```

## lambda 표현식 (임시로 쓰는 일회용 함수, 익명함수)
- 함수는 선언하기만 해도 RAM용량을 차지
- 1회만 사용하는 경우 lambda를 사용할 수 있음
```python
lambda parameter: expression(연산식)
```

## 타입힌트
- 개발자가 보기 편하게 참고하라고 주석을 달아놓은 것
- 변수에 타입힌트 (a: int, b:int)를 입력하거나, 출력 값의 타입을 입력해줌
    - my_sum(a, b) -> int:
- 정적언어: java 등, 상자 타입을 사전에 지정함
    - 개발은 번거롭지만 안정성이 높음
- 동적언어: 파이썬
    - 개발은 빠르지만 안정성이 떨어짐

## 이름공간(namespace), 스코프(scope)
- python에서 사용하는 이름들은 이름공간에 저장되어있음.
- LEGB 룰에 따라 접근 (작은 범위부터)
    - 1. Local: 정의된 함수 내부
    - 2. Enclosed: 상위 함수
    - 3. Global: 함수 밖
    - 4. Built-in: python이 기본적으로 가지고 있는 함수

## 재귀
- 함수 내부에서 자기 자신을 호출하는 함수
```python
n! = 1 * 2 * 3 * ... * n
1! = 1
2! = 1 * 2 = 1! * 2
3! = 1 * 2 * 3 = 2! * 3
n! = (n-1)! * n
```
#### (예) 피보나치 수열
- 중복되는 함수가 계속 반복되기 때문에 연산이 굉장히 오래 걸림
```python
def fib(n):
    if n == 0 or n == 1: # 첫번째 데이터가 0이고 두번째 데이터가 1이라면
        return 1 # 1을 반환해
    else:
        return fib(n-2) + fib(n-1)
```
