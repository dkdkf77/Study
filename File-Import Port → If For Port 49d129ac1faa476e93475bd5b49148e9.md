# File-Import Port → If For Port

```
num = 3

if num % 2 == 0:
    result = '짝수'
else:
    result = '홀수'

print(f'{num}은 {result}입니다.')

-output-
3은 홀수입니다.
```

이것을 간단하게 한줄로 만들수 있다 !

```
num = 3

result = **('짝수' if num % 2 == 0 else '홀수')**

print(f'{num}은 {result}입니다.')

-output-
3은 홀수입니다.
```

for문도 간단하게 만들 수 있다 !

```
a_list = [1,3,2,5,1,2]

b_list = []

for a in a_list:
    b_list.append(a*2)

print(b_list)

-output-

[2, 6, 4, 10, 2, 4]
```

이렇게 사용 

```
a_list = [1,3,2,5,1,2]

b_list = **[a*2 for a in a_list]**

print(b_list)

-output-
[2, 6, 4, 10, 2, 4]
```