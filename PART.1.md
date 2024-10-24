## 입력값

```python
a, b = map(int, input().split())

map(function, iter)  #map()은 여러 개의 데이터를 동시에 처리 
map(function, iter1, iter2)  #함수에 필요한 입력값이 두 개인 경우
```
***function*** : 각 요소에 적용할 함수, ***iter*** : 함수를 적용할 데이터 집합 <br/>

- 반복문 대신 한줄의 코드로 여러 개의 리스트 동시 처리 가능 > 가독성 증가
- 내부적으로 C로 구현되어 있어 Python 반복문보다 빠르게 처리 가능
- 새로운 리스트를 생성하지 않고, iterator 객체 반환 > 메모리 사용량 최소화 *(매우 큰 iterator 객체를 처리할 때는 메모리 사용량이 매우 높아질 수 있음 `*Why*`)*
