- `input()` : 일단 실행하고 이후에 들어오는 값을 넣어주세요.
    - 임의의 사용자가 직접 입력하길 원하는 경우

- `range(a, b, *c)` : a 부터 b-1까지 범위지정.
    - c값은 지정된 범위에서 c씩 떨어진 간격 지정.
    - c값은 음수로도 지정 가능 (감소)

- `enumerate()`: value 값의 인덱스 번호가 필요할 때 사용
```python
location = ['서울','대구','부산']
for location in enumerate(locations):
    print(location) 
# 출력
# (0, '서울')
# (1, '대전')
# (2, '부산')
# 나온 값은 []로 묶인 list가 아닌 tuple
```
- `dict(k_name='key', v_name='value')`: 딕셔너리 만들기
-  `dir(객체)`: 해당 객체가 사용할 수 있는 모든 속성과 매소드 리스트 반환
    - 만약 `dir('hello')`인 경우 스트링 객체가 가진 매소드 리스트 반환