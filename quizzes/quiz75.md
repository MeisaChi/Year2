# Quiz75 - Input to Binary Converter
## Code
```.py
ex1 = 'Hello World!'
ex2 = '42 is the answer.'
ex3 = 'ABC123'
def converter(data:str):
    converted = [str(bin(ord(i)))[2:] for i in data]
    string = ""
    for i in range(0, len(converted)):
        string = string + converted[i] + " "
    return string

print(converter(ex1))
print(converter(ex2))
print(converter(ex3))
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz75.png)

Fig.1 Pycharm's output from running the program
