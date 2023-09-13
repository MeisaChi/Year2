# Quiz77 - Parity Check
## Code
```.py
data = "100111001011001110010110011100101"
data2 = "011101111101110111110111001111"

def parity_checker(data):
    error = True
    state = "odd"
    if data[0]=='1':
        state = 'even'
    count = 0
    for i in range(1, len(data)):
        if data[i] == '1':
            count += 1
    if count%2 == 1 and state == 'odd' or count%2 == 0 and state == 'even':
        error = False
    return error

print(parity_checker(data))
print(parity_checker(data2))
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz77.png)

Fig.1 Pycharm's output from running the program
