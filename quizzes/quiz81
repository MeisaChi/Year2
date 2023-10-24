# Quiz81 - Name Collections
## Code
```.py
from collection import collection

a = collection()
temp_list = []

a.addItem('bob')
a.addItem('alice')
a.addItem('zoe')
a.addItem('roy')
a.addItem('john')
a.addItem('sam')
a.addItem('richard')


#put items in the list
a.resetNext()
while a.hasNext():
    item = a.getNext()
    temp_list.append(item)

print(temp_list)
#bubble sort
sort = True
while sort:
    sort = False
    for i in range(0,len(temp_list)-1):
        if temp_list[i][0]>temp_list[i+1][0]:
            temp = temp_list[i]
            temp_list[i] = temp_list[i+1]
            temp_list[i+1] = temp
            sort = True
        elif temp_list[i][0]==temp_list[i+1][0]:
            if temp_list[i][1] > temp_list[i + 1][1]:
                temp = temp_list[i]
                temp_list[i] = temp_list[i + 1]
                temp_list[i + 1] = temp
                sort = True

#put the list back on a new collection
b =  collection()
for t in temp_list:
    b.addItem(t)
print(b)
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz81.png)

Fig.1 Pycharm's output from running the program
