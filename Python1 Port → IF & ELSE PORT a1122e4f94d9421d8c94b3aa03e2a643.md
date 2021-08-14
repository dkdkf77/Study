# Python1 Port → IF & ELSE PORT

IF & ELSE 를 알아 보자 ! 

```
money = 3000

if money > 3800: **<- : 이 표시가 중요하다 !**
    print('택시를 타자')  **<- print문이 if 문에 속해져 있다는 뜻** 
else: **<- : 밑에 print 문이 else 문에 속해져 있다는 뜻**
    print('택시를 못타~')       <- 이 영역을 들여쓰기라고 한다고 튜터님이 말씀해주심

-output-
택시를 못타~
```

돈이 3800원 이상이면 '택시를 타자' output, 그게 아니면 '택시를 못타~' output

elif 문?

```
money = 1300

if money > 3800:
    print('택시를 타자')
elif money >1200:
    print('버스를 타자')
else:
    print('걸어가자')

-output-
버스를 타자
```

다른 선택지를 주는 건가? ㅎㅎ if문은 쉬웠지만 알고리즘은 holy moly 일듯 .. ㅎㅎ