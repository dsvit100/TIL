
- if num % 2 는 if num % 2 != 0 과 같다
    - **질문**
    - if num % 2: 이게 왜 if num % 2 != 0 과 같은지?
    - num = 4인 경우
    - if 4 % 2 의 값은 0, False
    - num = 5인 경우
    - if 5 % 2 의 값은 1, True
```python
num = int(input())

if num % 2: # 만약 num이 2로 나눴을 때 나머지가 0인 경우(False인 경우)
        print('odd')
else:
    print('even')
```
