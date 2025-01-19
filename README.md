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


## 4️⃣ find()

```문자열.find(검색 대상)```
- 문자열에 사용하는 메소드
- 문자열 내에서 찾고자하는 문자의 인덱스를 반환

### 예시
```python
str = "findletter"
print(str.find("d"))
```

## 5️⃣ EOFError

```EOF > End Of File```
- while문에서 더 이상 읽을 파일이 없을 때 발생하는 에러
- try / except을 사용하여 해결

### 예시
```python
import sys

while True:
    try:
        a = int(input())
        if a == 0:
            break
        print(a)

    except EOFError:
        break
```

## 6️⃣ replace()

```str = str.replace(replace 할  대상, 어떤 것으로 replace 할 지)```
- 문자열에서 특정 부분을 특정 문자로 치환하기 위해 사용하는 메소드

### 예시
```python
str = str.replace(a, "X") #str에서 a를 모두 X로 바꿈꿈
```