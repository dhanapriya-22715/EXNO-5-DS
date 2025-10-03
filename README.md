
# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
```
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x = [2018, 2019, 2020, 2021, 2022]
y = [15000, 20000, 25000, 30000, 35000]

plt.plot(x, y, 'g*', linestyle='dashed', linewidth=2, markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```

<img width="1041" height="588" alt="image" src="https://github.com/user-attachments/assets/8c35393e-6d73-4359-bfbf-1ef06aad4dc9" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'--')
plt.subplot(2,2,2)
plt.plot(x,y,'o--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
plt.show()

```

<img width="883" height="531" alt="image" src="https://github.com/user-attachments/assets/8442fd75-9c32-4c3c-9395-866cc9867215" />


```
x = np.arange(0, 4*np.pi, 0.1)
y = np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()

```

<img width="1014" height="555" alt="image" src="https://github.com/user-attachments/assets/22c331bf-3dbe-4b19-922d-9b6490bf4e49" />

```
x = [2, 8, 10]
y = [11, 16, 9]
x1 = [3, 4, 11] 
y1 = [6, 15, 7]
plt.bar(x, y, color='r')
plt.bar(x1, y1, color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()

```

<img width="1006" height="581" alt="image" src="https://github.com/user-attachments/assets/6381e49d-3f1c-4d27-9de6-648185ed3e82" />

```
x = [1, 2, 3]
y = [7, 3, 9]

plt.plot(x, y, color='g')
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()

```

<img width="893" height="586" alt="image" src="https://github.com/user-attachments/assets/01193bb3-c962-4253-bff9-30b657a16832" />

```
x1 = [1, 2, 3]
y1 = [2, 4, 1]
plt.plot(x1, y1, label='line1')

x2 = [1, 2, 3]  
y2 = [4, 1, 3]
plt.plot(x2, y2, label='line2')

plt.title("multiline graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()

```

<img width="983" height="580" alt="image" src="https://github.com/user-attachments/assets/9a482246-a83b-4461-b0c3-11cfaaa9f3fe" />

```
x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth=3, 
         marker='o', markerfacecolor='red', markersize=12, label='spices')
plt.xlim(1, 8)
plt.ylim(1, 8) 
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()

```

<img width="957" height="581" alt="image" src="https://github.com/user-attachments/assets/730431ed-b51d-4461-b90c-87166cad99ee" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.931]
plt.plot(yield_apples,linestyle='dashed',linewidth=3,marker='*',markersize=12,color='g')
plt.show()

```

<img width="1019" height="529" alt="image" src="https://github.com/user-attachments/assets/4eae7d29-5395-4591-919e-4e9e28bb7762" />


```
oranges = [2, 4, 6, 7, 8, 12, 45]
apples = [2, 4, 5, 6, 8, 23, 37]
years = [2019, 2020, 2021, 2022, 2023, 2024, 2025]
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='*')
plt.title('Crop yields in Kanto')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.legend(['apples', 'oranges'])  
plt.show()

```

<img width="889" height="584" alt="image" src="https://github.com/user-attachments/assets/f6889d4e-62ac-4dd6-8adf-090fc3028481" />

```

oranges = [2, 4, 6, 7, 8, 12]
apples = [2, 4, 5, 6, 8, 23]
years = [2019, 2020, 2021, 2022, 2023, 2024]
plt.bar(oranges,apples)
plt.plot(years, apples, label='apples', marker='*')
plt.plot(years, oranges, label='oranges', marker='o')
plt.title('Fruit sales')  
plt.xlabel('Year')  
plt.ylabel('Sales')  
plt.legend()  
plt.show()

```

<img width="906" height="578" alt="image" src="https://github.com/user-attachments/assets/ea8aee37-53d2-4a6e-9012-a0c21e888000" />

```
plt.figure(figsize=(12,6))
plt.plot(years, oranges, marker='o',label='oranges')
plt.title("yield of oranges (tons per hectare)")
plt.legend()

```

<img width="1240" height="714" alt="image" src="https://github.com/user-attachments/assets/74dc57b1-7211-4cad-a685-a4e7a05241b3" />

```

import matplotlib.pyplot as plt
print("scatter plot is:")
x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
y = [2, 4, 5, 7, 6, 8, 9, 11, 12, 12]
plt.scatter(x, y, label='star', color='green', marker='*', s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()

```

<img width="939" height="619" alt="image" src="https://github.com/user-attachments/assets/a274a21e-3657-46a0-8234-bc4584ebd1ae" />

```

import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='green',label='y1')
plt.fill_between(x, y2, color='blue', label='y2')
plt.fill_between(x, y3, color='red',label='y3')
plt.title("Fill Between Example")
plt.legend()
plt.show()

```

<img width="889" height="562" alt="image" src="https://github.com/user-attachments/assets/cb754789-77b2-4e4d-90fc-1fa4d66a9b37" />


```
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()

```

<img width="934" height="562" alt="image" src="https://github.com/user-attachments/assets/9a2848dc-db7b-4f22-90ee-1e05514d1f4f" />


```

from scipy.interpolate import make_interp_spline
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 9, 10, 11, 12, 13])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.show()

```

<img width="839" height="532" alt="image" src="https://github.com/user-attachments/assets/f4bf24b3-50ae-43e3-8285-7de7f3b5406b" />

```

values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()

```
<img width="942" height="527" alt="image" src="https://github.com/user-attachments/assets/d9abe1db-468c-42cb-bd02-3a6440000c59" />

```

ages = [2, 5, 70, 40, 45, 50, 43, 40, 44, 60, 7, 13, 57, 18, 90, 77, 32, 21, 20, 40]
range1 = (0, 100)
bins = 10
plt.hist(ages, bins, range1, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no. of people')
plt.title('my histogram')
plt.show()

```

<img width="943" height="581" alt="image" src="https://github.com/user-attachments/assets/05173d25-896d-44f9-90d0-ae5762cfe8b7" />

```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='green',alpha=0.5)
plt.show()

```

<img width="859" height="531" alt="image" src="https://github.com/user-attachments/assets/a5543fab-28a1-4185-b8ff-0d57a24f649a" />

```

np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data

```

<img width="953" height="434" alt="image" src="https://github.com/user-attachments/assets/c213500c-855e-4971-9ed8-8a40922c0544" />

```

fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')

```

<img width="931" height="623" alt="image" src="https://github.com/user-attachments/assets/d9df9513-60a3-4ca7-825d-d58044ca9600" />

```

activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6]
colors=['y', 'g', 'b', 'r']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1,0), radius=1.2, autopct="X1.1")
plt.legend()
plt.show()

```

<img width="1192" height="517" alt="image" src="https://github.com/user-attachments/assets/83b0f78f-614e-4fdb-b85d-f31a7abce57e" />

```
labels='python', 'C+', 'ruby', 'java'
sizes=[215,130,245,210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, colors=colors, labels=labels, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()

```

<img width="938" height="497" alt="image" src="https://github.com/user-attachments/assets/c5412576-40e6-4a6a-9eea-fe3874c0c776" />

# Result:

Thus,all the data visualization techniques of matplotlib  has been implemented.

