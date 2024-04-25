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
```
NAME: PRIYANKA A
REG NO: 212222230113
```
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

<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/509b5107-55e6-4900-a34a-f5fe33d0b05f" width="300" height="300">
<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/35ac1abf-13c4-420d-a20c-c5117565962a" width="300" height="300">

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

<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/fa9fac25-8e8c-4062-b404-c4059b83acf3" width="300" height="300">
<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/fcbb4cad-b588-44bc-817f-c6a36c6f3ffe" width="300" height="300">


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


<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/ba4816f7-a5ca-43ae-ab56-704ed464e76a" width="300" height="300">
<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/8c753a88-9da7-495d-9842-88dac5ab9a93" width="300" height="300">


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

<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/c59b9cd9-fd38-425e-97ee-9de8c42674dd" width="300" height="300">



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

<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/1193c6a0-ec5b-42ed-a6ac-118136f3b671" width="300" height="300">



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```


<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/5355375e-9777-4bc8-83c1-cae6d2da9c2a" width="300" height="300">



### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```


<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/6b540f13-933a-4cf4-8923-eeb8642ffbb2" width="300" height="300">


```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img src="https://github.com/PriyankaAnnadurai/EXNO-5-DS/assets/118351569/4e6304ff-5a0b-49bd-be9a-45798994d467" width="300" height="300">





## Result:

Thus, all the data visualization techniques of matplotlib has been implemented.
