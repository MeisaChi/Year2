# Quiz70
## Code
```.py
iplist = []
a,b,c,d, = 0,0,0,0
for ip in range((256**4)-256,256**4):
    a = ip%256
    b = (ip//256)%256
    c = ((ip // 256)//256) % 256
    d = (((ip // 256) // 256)//256) % 256
    iplist.append(f"{d}.{c}.{b}.{a}")
print(iplist)
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz70.png)
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz70-2.png)
