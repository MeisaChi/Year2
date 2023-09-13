# Quiz76 - Error Checker
## Code
```.py
data = "100111001011001110010110011100101"
data2 = "011101111101110111110111001111"

def error_check(data):
    error = False
    original = data[0:len(data)//3]
    copy1 = data[len(data)//3:2*len(data)//3]
    copy2 = data[2*len(data)//3:len(data)]
    if copy1 != copy2 or copy1 != original:
        error = True
    return error

print(error_check(data))
print(error_check(data2))
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz76.png)

Fig.1 Pycharm's output from running the program
