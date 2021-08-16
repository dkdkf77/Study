# Tuple Port → F-String Port

```
scores = [
    {'name':'영수','score':70},
    {'name':'영희','score':65},
    {'name':'기찬','score':75},
    {'name':'희수','score':23},
    {'name':'서경','score':99},
    {'name':'미주','score':100},
    {'name':'병태','score':32}
]

for s in scores:
    name = s['name']
    score = s['score']
    **print(name+'의 점수는 '+str(score)+'점 입니다.')**

-output-
영수의 점수는 70점 입니다.
영희의 점수는 65점 입니다.
기찬의 점수는 75점 입니다.
희수의 점수는 23점 입니다.
서경의 점수는 99점 입니다.
미주의 점수는 100점 입니다.
병태의 점수는 32점 입니다.
```

딕셔너리에 자료가 많으면 print 문에 적을게 많아 지는데 

```
scores = [
    {'name':'영수','score':70},
    {'name':'영희','score':65},
    {'name':'기찬','score':75},
    {'name':'희수','score':23},
    {'name':'서경','score':99},
    {'name':'미주','score':100},
    {'name':'병태','score':32}
]

for s in scores:
    name = s['name']
    score = s['score']
    print(**f'{name}**의 점수는 **{score}점**입니다.')
```

이런 식으로 **f-string을 사용**하면 간략하게 똑같은 문장을 출력 할 수 있다 !