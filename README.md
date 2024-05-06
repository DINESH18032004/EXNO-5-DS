# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:


> Developed By: DINESH KUMAR R

> REG NO: 212222110010
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/65a473de-15a0-4c4b-8791-2c35ee7000c0)![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/0b97fa05-9adf-4eb0-a80a-6ff06479e0ff)



### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/18ce4479-3cdd-4d30-b488-3ead72a56ebc)![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/b761fff0-050f-49ad-9bee-7e483c4cec68)




### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```


![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/21c44779-e972-4c76-a911-e61fd754e0e7)![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/92ee2b6a-4181-45ad-9e4d-454f50fd6c91)




### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/3c912523-53b5-497e-9300-ed7755b59fc6)




### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/45f0aabc-65fa-4521-809d-64e5a435428b)



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/096b1764-9d80-420a-98a5-c13fd7a5a024)




### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/33616c18-9c6d-432a-b7a0-c13a5860f50c)



```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/DINESH18032004/EXNO-5-DS/assets/119477784/56a98139-561b-4fba-b838-43d155e01671)



## Result:

### Thus, all the data visualization techniques of matplotlib has been implemented.
