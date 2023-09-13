# Quiz72 - MAC Generator
## Code
```.py
from random import randint

N = 7

def HexGen():
    num = ""
    a = randint(0,15)
    let = ['A','B','C','D','E','F']
    if a >= 10:
        num += let[a-10]
    else:
        num = a
    return num

list = []
for a in range (0,N):
    set = ""
    aaa = 6
    while aaa > 0:
        stri = ""
        for a in range (0,2):
            stri += str(HexGen())
        if stri not in set:
            if aaa > 1:
                set += stri
                set+= ":"
                aaa = aaa-1
            else:
                set += stri
                aaa = aaa - 1
        else:
            pass

    list.append(set)
print(list)
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz72.png)

Fig.1 Pycharm's output from running the program
