# Bon-Voyage! Rapha port → python1

문자열 **Quiz**

- 10) ✍️ Q. 문자열의 앞의 반만 출력하기

    `"sparta"`의 앞의 3글자인 `"spa"`만 출력해봅시다.

    - A.  풀이

        ```python
        text = "sparta"
        print(text[:3])
        ```

- 11) ✍️ Q. 전화번호의 지역번호 출력하기

    ```python
    phone = "02-123-1234"
    ```

    힌트: `.split()`을 써보세요!

10) 풀이

```
txt = 'Raphael'

result = txt[**:3**]

print(result)
```

11) 풀이

```
num = '051-842-9900'

result = num**.split('-')[0]**

print(result)
```

list 를 배워 봅시다 ! 알렐루야 !!! 아멘!!! 응?

```
a_list = [2, '배', True, ['사과','감']]
print(a_list)
```

이처럼 list 안에는 숫자, 문자, 참 or 거짓, 또 다른 리스트 가  올수도 있다.

또 다른 list 안에 문자('감')를 output 하고 싶을 때!

```
a_list = ['사과','배','감',['사과',**'감'**]]

print(a_list**[3][1]**)

-output-
감
```

list에 추가 하고 싶을 때 

```
a_list = [1,5,2,345,6,2]

a_list**.append**(99)

print(a_list)

-output-

[1,5,2,345,6,2,99]
```

→ .append 안에 2개를 추가 해 보았다.

```
a_list = [1,5,2,345,6,2]

a_list**.append(99,100)**

print(a_list)

-output-
**TypeError: append() takes exactly one argument (2 given)**
```

**append 에 2개를 넣는 것은 안되는 것 같다.**

list도 문자열 처럼 나눠서 출력이 가능 하다한다

```
a_list = [1,5,2,345,6,2]

result = a_list[:4]

print(result)

-output-

[1,5,2,345]
```

문자열 및 list에서 제일 마지막 문자 및 숫자를 출력 하는 방법

```
a_list = [1,5,2,345,6,2,9]

result = a_list[-1]

print(result)

-output-
9
```

**물론, a_list[6]으로도 출력 가능 하지만 [-1]을 사용하니 무조껀 마지막 숫자가 출력 되는 것을 확인 하였다.** 

리스트 안에 길이(갯수)를 구하는 방법 

```
a_list = [1,5,2,345,6,2,9]

result = **len**(a_list)

print(result)

-output-

7
```

이번 꺼는 튜터 님이 재미있는 거라는데 얼마나 재미있나 보자..

```
a_list = [1,5,2,345,6,2,9]

**a_list.sort()**

print(a_list)

-output-
[1, 2, 2, 5, 6, 9, 345]
```

신선 했다 👍   >밑에는 꺼꾸리 숫자 

```
a_list = [1,5,2,345,6,2,9]

a_list.sort(**reverse=True**)

print(a_list)

-output-
[345, 9, 6, 5, 2, 2, 1]
```

알고리즘 ! 문제를 풀 때 사용 된단다 

list안에 문자가 있는 지 찾고 싶을 때 ?

```
a_list = [1,5,2,345,6,2,9]

result = (5 in a_list)

print(result)

-output-
True
```

Dictionary ? 이거 철자 맞나? 아무튼 딕셔너리 를 배워보자 ! 

```
a_dict = {'name':'rapha','age':'비밀'}

print(a_dict['name'])

-output-

rapha
```

이름과 나이만 되는 줄 알았는데 ? > 밑에 처럼 리스트도 된다!

```
a_dict = {'name':'rapha','age':'비밀','friend':['협꼬','훈꼬','은꼬','광꼬']}

print(a_dict['friend'])

-output-
['협꼬', '훈꼬', '은꼬', '광꼬']
```

문자열 과 리스트 와는 다르게 간단하게 추가를 할 수 가 있다

```
a_dict = {'name':'rapha','age':'비밀','friend':['협꼬','훈꼬','은꼬','광꼬']}

**a_dict['height'] = 183**

print(a_dict)
```

딕셔너리 안에 height가 있는 지 확인 하는 방법!

```
a_dict = {'name':'rapha','age':'비밀','friend':['협꼬','훈꼬','은꼬','광꼬']}

print(**'height' in a_dict**)
```

별표!> list 와 dict의 조합 

```
people = [{'name':'rapha','age':'비밀'},{'name':'gabri','age':'??'}]

**print(people[1]['age'])**

-output-

??
```

list 안에 dict 2개 포함 되어 있는 형태로 1번째 딕셔너리에 age를 output 하는 type

list & dict Quiz! 

smith의 science 점수를 출력해보세요

```
people = [
    {'name': 'bob', 'age': 20, 'score':{'math':90,'science':70}},
    {'name': 'carry', 'age': 38, 'score':{'math':40,'science':72}},
    {'name': **'smith'**, 'age': 28, 'score':{'math':80,**'science':90**}},
    {'name': 'john', 'age': 34, 'score':{'math':75,'science':100}}
]
```

문제 풀이 

```
people = [
    {'name': 'bob', 'age': 20, 'score':{'math':90,'science':70}},
    {'name': 'carry', 'age': 38, 'score':{'math':40,'science':72}},
    {'name': 'smith', 'age': 28, 'score':{'math':80,'science':90}},
    {'name': 'john', 'age': 34, 'score':{'math':75,'science':100}}
]

print(people[**2**]['**score**']['**science**'])
```

하고 싶은 말은 리스트 안에 딕셔너리가 있다는 건가?