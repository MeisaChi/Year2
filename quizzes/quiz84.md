# Quiz84 - Number Classes
## Code
```.py
cclass fourDigitNumber:
    def __init__(self, value):
        self.intValue = value
        self.thouDigit = self.intValue //1000
        self.hundDigit = self.intValue % 1000 //100
        self.tensDigit = self.intValue % 1000 % 100 //10
        self.onesDigit = self.intValue % 1000 % 100 % 10

    def getNumbers(self):
        return (self.thouDigit, self.hundDigit, self.tensDigit, self.onesDigit)

test = fourDigitNumber(value=2312)
test2 = fourDigitNumber(value=5769)
print(test.getNumbers())
print(test2.getNumbers())
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz84.png)

Fig.1 Pycharm's output from running the program
