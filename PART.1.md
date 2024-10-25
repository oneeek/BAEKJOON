## 사칙연산(10869)

-  [x] 제출코드
```python
a,b = map(int, input().split())
print(a+b, a-b, a*b, a//b, a%b, sep='\n')
```

-  [x] 📝
```python
문자열.split()  #띄어쓰기를 기준으로 문자열 나누기 
문자열.split('구분자')  #구분자를 기준으로 문자열 나누기
```

```python
map(function, iter)  #iter(반복가능객체)에 function(함수)을 동시에 처리
map(function, iter1, iter2)  #function의 입력값이 두 개인 경우
```
- 반복문 대신 한줄의 코드로 처리 가능 ▶ 가독성 증가
- 내부적으로 C로 구현되어 있어 Python 반복문보다 빠르게 처리 가능
- 지연평가(lazy evaluation) 방식 ▶ 효율적인 메모리 사용과 성능 최적

-  [X] 
> **지연평가(lazy evaluation)**
> iterator는 값을 차례대로 꺼낼 수 있는 객체로, 데이터를 미리 만들어두지 않고 필요한 시점이 되었을 때 데이터를 생성
> 필요할 때만 값을 계산하여 불필요한 계산 방지


##
