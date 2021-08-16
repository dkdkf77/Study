# If-For Port → Map-Filter-Lamda Port

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

def check_adult(person):
    if person['age'] > 20:
        return '성인'
    else:
        return '청소년'

result = **map(check_adult, people)**

print(list(result))
```

map = people을 돌면서 check_adult 를 map  해주서 list에 감싼 것 

뭔 말이지..

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

def check_adult(person):
    **return('성인' if person['age'] > 20 else '청소년')**

result = map(check_adult, people)

print(list(result))
```

윗 쪽 꺼를 간략하게 써준것 

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

result = map(lambda person : ('성인' if person['age'] > 20 else '청소년'), people)

print(list(result))
```

lambda를 사용하여 더 간략히 써 줄 수 있다. 이거는 쪼금 어렵네 ...

filter를 사용

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

result = **filter**(lambda person: person['age'] > 20, people)

print(list(result))
```

오히려 더 쉽고 간단해서 많이 사용 될수도 있다고 한다.

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

result = filter(lambda x: x['age'] > 20, people)

print(list(result))
```