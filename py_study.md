# 끝이 없는 Python
문제 풀이 및 솔루션 / 스터디를 통해 새롭게 알게 되었거나, 공부한 정보들을 정리해둔 공간

## 1️⃣ split()과 map()

> split()

```문자열.split()```
- 값을 여러 개 입력받고 정수, 실수로 변환
- 문자열 리스트이기에 map 이용 가능

> map()

```map(적용할 함수, 함수를 적용할 데이터 집합)```
- 리스트의 요소를 지정된 함수로 처리해주는 함수

### 예시
```python
a, b = map(int, input().split())
# a, b의 값을 각각 받지 않고 split() 함수를 통해 한번에 input 받기
# 입력 받은 값들을 map() 함수를 통해 int의 형태로 각각 저장
```

## 2️⃣ join()

> join()

```"구분자".join(리스트)```
- 매개변수로 들어온 리스트에 있는 요소 하나하나를 합쳐서 하나의 문자열로 바꾸어 반환하는 함수

### 예시
```python
        first = "".join(reversed(word[:i]))
        second = "".join(reversed(word[i:j]))
        third = "".join(reversed(word[j:]))

        answer.append(first + second + third)
```

## 3️⃣ sort()와 sorted()의 차이점

> sort()

```리스트명.sort()```
- list형의 메소드(method)
- list 원본값을 직접 수정

> sorted()

```sorted(리스트명)```
- 내장 함수
- list 원본값은 그대로이고, 정렬값을 반환