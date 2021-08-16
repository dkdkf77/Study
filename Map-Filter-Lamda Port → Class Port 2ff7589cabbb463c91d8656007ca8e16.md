# Map-Filter-Lamda Port → Class Port

```
class  monster():
    hp = 100
    alive = True

    def damage(self, attack):
           self.hp = self.hp - attack
           if self.hp < 0:
               self.alive = False

    def status_check(self):
        if self.alive == True:
            print('살았다')
        else:
            print('죽었다')

m1 = monster()
m1.damage(150)
m1.status_check()

m2 = monster()
m2.damage(90)
m2.status_check()

-output-
죽었다
살았다
```

각각의 몬스터의 객체화 시킬때 사용 ! ㅎㅎ

⭐ **튜터님의 말씀! 파이썬은 방대한 언어를 가지고 있으므로 아직 안 배운게 많지만 우리에게는 구글링이 있다. 너무 걱정말아라 그리고 외우려고 하지 마라 미련한 짓이다.  계속 쓰다보면 자동적으로 익숙해진다 한다.**