# If & Else Port → For Port

For문의 기본 형식

```
Chinese_food = ['짜장면','짬뽕','탕수육','양장피','팔보체','꿔봐로우']

for ccangge in Chinese_food:
    print(ccangge)

-output-

짜장면
짬뽕
탕수육
양장피
팔보체
꿔봐로우
```

For 문은 반복되는 문장을 간략 하게 output 해준다 ! 

For문 예제 ! 

```python
people = [
    {'name': 'bob', 'age': 20},
    {'name': 'carry', 'age': 38},
    {'name': 'john', 'age': 7},
    {'name': 'smith', 'age': 17},
    {'name': 'ben', 'age': 27},
    {'name': 'bobby', 'age': 57},
    {'name': 'red', 'age': 32},
    {'name': 'queen', 'age': 25}
]
```

이 리스트에서 나이가 20보다 큰 사람만 출력합니다.

**내가 풀은 방식;;;;; 아 ... 아직 멀었나 보다 ㅎㅎ**

```
people = [
    {'name': 'bob', 'age': 20},
    {'name': 'carry', 'age': 38},
    {'name': 'john', 'age': 7},
    {'name': 'smith', 'age': 17},
    {'name': 'ben', 'age': 27},
    {'name': 'bobby', 'age': 57},
    {'name': 'red', 'age': 32},
    {'name': 'queen', 'age': 25}
]

for person in people:
        if person > 20:
            print(person['age'])

```

풀이 과정 ! 

```
people = [
    {'name': 'bob', 'age': 20},
    {'name': 'carry', 'age': 38},
    {'name': 'john', 'age': 7},
    {'name': 'smith', 'age': 17},
    {'name': 'ben', 'age': 27},
    {'name': 'bobby', 'age': 57},
    {'name': 'red', 'age': 32},
    {'name': 'queen', 'age': 25}
]

for person in people:
        name = person['name']
        age = person['age']
        if age > 20:
            print(name)
```

i 와 enumerate 사용법 

i는 for 문 안에 순서를 매겨 준다 

```
people = [
    {'name': 'bob', 'age': 20},
    {'name': 'carry', 'age': 38},
    {'name': 'john', 'age': 7},
    {'name': 'smith', 'age': 17},
    {'name': 'ben', 'age': 27},
    {'name': 'bobby', 'age': 57},
    {'name': 'red', 'age': 32},
    {'name': 'queen', 'age': 25}
]

for **i**, person in enumerate(people):
    name = person['name']
    age = person['age']
    print(i, name, age)

-output-
**1** carry 38
**2** john 7
**3** smith 17
**4** ben 27
**5** bobby 57
**6** red 32
**7** queen 25
```

i를 빼고 쳤더니 오류가 나온다

break 사용

```
for i, person in enumerate(people):
    name = person['name']
    age = person['age']
    print(i, name, age)
    **if i > 3
        break**

-output-
0 bob 20
1 carry 38
2 john 7
3 smith 17
**4** ben 27
```

i 가 3보다 커지면 break 를 걸어 output

별표> 이것을 사용하는 이유는 코딩을 처음 시작시  리스트가 만줄정도가 될때 i와 enumerate 그리고 break를 사용하여 간략하게 디버깅을 하게 사용