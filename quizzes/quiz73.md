# Quiz73 - MAC and IP table
## Code
```.py
class ip_generator():
    def __init__(self):
        self.num = 1
        self.mac_table = []
        self.ip_table = []
    def new_ip(self, data):
        if self.ip_table==[]:
            self.ip_table.append(f"192.168.0.{self.num}")
            self.mac_table.append(data)
            self.num += 1
        else:
            ind = -1
            for i in range(len(self.mac_table)):
                if data == self.mac_table[i]:
                    ind = i
            if ind == -1:
                self.ip_table.append(f"192.168.0.{self.num}")
                self.mac_table.append(data)
                self.num += 1
            else:
                self.ip_table.append(self.ip_table[ind])
                self.mac_table.append(data)

gen = ip_generator()
while True:
    abc = input()
    gen.new_ip(abc)
    for i in range(len(gen.ip_table)):
        print(f"{gen.mac_table[i]} | {gen.ip_table[i]}")
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz73.png)

Fig.1 Pycharm's output from running the program
