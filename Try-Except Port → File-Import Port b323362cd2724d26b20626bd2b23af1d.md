# Try-Except Port → File-Import Port

다른 파일에 있는 내용을 불러 올고 싶을 때 !

```
def say_hi():
    print('안녕!')

def say_hi_to(name):
    print((f'{name}님 안녕하세요!'))
```

다른 파일에서 from, import를 사용 하여 불러 올수 있다 !

```
from main_func import *

say_hi()
say_hi_to('영수')
```

**⭐ 중요한 것은 파일 명에 ' . ' 을 붙이면 인식을 못한다!**