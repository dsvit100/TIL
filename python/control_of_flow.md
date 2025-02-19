# 제어문
- 방향을 제안함

## 조건문 (if문)
- if문은 반드시 참/거짓을 판단할 수 있는 `조건식`과 함께 사용
    - `if <조건식>`
- <조건식>이 참인 경우 : `:` 이후의 문장을 실행
- <조건식>이 거짓인 경우 : `else:` 이후의 문장을 실행

```python
if <조건식>:
# if의 조건식이 참인 경우 실행할 코드
else:
# if의 조건이 거짓인 경우 실행할 코드
```

### elif (else & if)
```python
if <조건식>:
    if문이 참인 경우 - 이 조건 맞아?
elif <조건식>:
    elif문이 참인 경우 - 1, 2, 3...개의 조건은 맞아?
else:
    위의 모든 조건식이 거짓인 경우
```

### 조건표현식
```python
true_value if <조건식> else false_value
# 참인경우 true_value 값을, 거짓인 경우 false_value 값을 출력

(예)
num = 9
result = '홀수' if num % 2 else '짝수'
# 만약 num % 2의 값이 1(True)이라면 홀수, 0(False)라면 짝수로 표현
```

## 반복문
### while문
- 조건식이 참인 동안에는 반복, 거짓인 경우 stop
```python
while <조건식>:
    실행할 코드

(예)
a = 0
while a < 5: # a가 5보다 작으면 계속 반복할거야
    a += 1 # a(현재 0)에 1씩 더해줘 -> while문 반복, a가 5가 될 때까지
    print(a)
```

### for문
- 정해진 범위 내의 반복
```python
for var_name in sequnce(리스트, 튜플, 레인지, 스트링):
    code
```

### dictionary 반복
```python
info = {
    'name': 'gildong',
    'location': 'seoul',
    'phone': '010-1234-1234',
    'age': 20
}

- 1. for key in dict
    - `for k in info` : key 출력
    - # 출력값: name \n location \n phone \n age
- 2. for key in dict.keys()
    - `for k in info.keys()` : key와 value 출력
    - # 출력값: name \n gildong \n location \n seoul ...
- 3. for value in dict.values()
    - `for v in info.values()` : value 출력
    - # 출력값: gildong \n seoul \n 010-1234-1234 ...
- 4. for key, value in dict.items()
    - `for k, value in info.items()`
        : print(k, v) 실행, key와 value가 각 key에 따라 줄바꿈으로 출력됨
    - # 출력값: name gildong \n location seoul \n ...
```

### break
- 반복문을 종료시키는 키워드

### continue
- continue 이후의 코드를 실행하지 않고 다음 반복을 진행
    - 특정 상황에서 스킵하고 계속 진행할 때 사용

### else
- else문은 끝까지 반복된 경우 실행됨 (break를 만나지 않은 경우 실행)
- break를 통해 반복이 강제종료되면 else는 출력되지 않음