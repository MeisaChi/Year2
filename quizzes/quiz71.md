# Quiz71 - IPv6 Generator

## Code
```.py
from random import randint

def hextonum(s):
    letter = ['A', 'B', 'C', 'D', 'E', 'F']
    if s >= 10:
        x = s-10
        con = letter[x]
        return con
    else:
        return s

N = 7

address = []

for input in range (0,N):
    ipv6 = ""

    for x in range (0,8):
        string = ""

        for y in range (0,4):
            s = randint(0,15)
            string += str(hextonum(s))

        if x != 7:
            ipv6 += string
            ipv6 += ":"

        else:
            ipv6 += string

    address.append(ipv6)
print(address)
```

## Evidence
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz71.png)

Fig.1 Pycharm's output from running the program
