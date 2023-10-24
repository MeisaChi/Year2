# Quiz85 - Employee Classes
## Code
```.py
class citizen:
    def __init__(self, name, city, status):
        self.name = name
        self.city = city
        self.status = status

    def getName(self):
        return(self.name)

    def getCity(self):
        return(self.city)

    def getStatus(self):
        return(self.status)

class employee(citizen):
    def __init__(self, name, city, status, salary):
        self.salary = salary
        super().__init__(name,city,status)

    def getSalary(self):
        return(self.salary)

class partTimeEmployee(employee):
    def __init__(self, name, city, status, salary, realNumber, union):
        self.realNumber = realNumber
        self.union = union
        super().__init__(name,city,status,salary)

bob = citizen('bob','tokyo','alive')
alice = employee('alice','kyoto','Alive',100000)
dice = partTimeEmployee('dice','nagano','alive',50000,0.5,False)
print(bob.getName(),bob.getCity(),bob.getStatus())
print(alice.getName(),alice.getCity(),alice.getStatus(),alice.getSalary())
print(dice.getName(),dice.getCity(),dice.getStatus(),dice.getSalary())
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz85.png)

Fig.1 Pycharm's output from running the program
