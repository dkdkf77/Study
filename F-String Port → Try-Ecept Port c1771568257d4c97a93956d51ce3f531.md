# F-String Port → Try-Ecept Port

```
people = [
    {'name': 'bob', 'age': 20},
    {'name': 'carry', 'age': 38},
    {'name': 'john', 'age': 7},
    {'name': 'smith', 'age': 17},
    {'name': 'ben', 'age': 27},
    {'name': 'bobby'},
    {'name': 'red', 'age': 32},
    {'name': 'queen', 'age': 25}
]

for person in people:
    if person['age'] > 20:
            print(person['name'])

-output- 
Traceback (most recent call last):
  **File "/Users/lyuseunghwan/Desktop/sparta_python/hello.py", line 13, in <module>
    if person['age'] > 20:
KeyError: 'age'**
carry
ben
```

bobby의 age가 없어서 age가 비어 있다고 error가 output

이럴 때 

```
people = [
    {'name': 'bob', 'age': 20},
    {'name': 'carry', 'age': 38},
    {'name': 'john', 'age': 7},
    {'name': 'smith', 'age': 17},
    {'name': 'ben', 'age': 27},
    **{'name': 'bobby'},**
    {'name': 'red', 'age': 32},
    {'name': 'queen', 'age': 25}
]

for person in people:
    **try:**
        if person['age'] > 20:
             print(person['name'])

    **except:**
        **print('에러입니다')-> ex> print(person['name'], '에러입니다') 를 사용해주면 어디서 에러가 났는지 알수 있다.

-output-**

carry
ben
**에러입니다 -> ex> bobby 에러입니다**
red
queen
```

많은 자료를 처리 하다 error로 인해 자료가 다 날라 가지 말라고 사용해준다고 한다.

**왠만하면 안쓰는게 좋다고 한다 !**