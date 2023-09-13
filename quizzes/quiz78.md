# Quiz78 - Port Checker
## Code
```.py
data1 = '100111001011001110010110011100101'
data2 = '10101100110101111110111001111'
data3 = '000000000101000011001011'

def Layer4_firewall(data):
    filtered = True
    portnum = 0
    msg = None
    msg2 = None
    index = 0
    for i in range (15,0,-1):
        if data[i] == '1':
            portnum += 2**index
        index += 1
    if portnum == 80 or portnum == 22123:
        filtered = False
        msg = data[16:len(data)]
        msg2 = f"Port number is {portnum}"
    return filtered, msg, msg2

print(Layer4_firewall(data1))
print(Layer4_firewall(data1))
print(Layer4_firewall(data3))
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz78.png)

Fig.1 Python's output from running the program
