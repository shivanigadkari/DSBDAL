# DSBDAL-ASS-1

Q1]
import numpy as np 
runs = np.array([    [45, 50, 30, 60, 25],    [10, 15, 5, 20, 12],    [80, 60, 75, 100, 90],    [25, 30, 20, 35, 40],    [0, 5, 10, 0, 2],    [50, 55, 60, 65, 70],    [35, 40, 45, 50, 55],    [100, 110, 120, 115, 125],    [10, 12, 15, 10, 8],    [70, 80, 85, 90, 95],    [40, 45, 50, 55, 60] ])
x=np.sum(runs)
x
o/p:2664

Q2]
x=np.max(runs[0])
x
o/p:60

Q3]
x=np.mean(runs[0])
x
42.0
x=np.mean(runs[1])
x
12.4
x=np.mean(runs[2])
x
81.0
x=np.mean(runs[3])
x
30.0
x=np.mean(runs[4])
x
3.4
x=np.mean(runs[5])
x
60.0
x=np.mean(runs[6])
x
45.0
x=np.mean(runs[7])
x
114.0
x=np.mean(runs[8])
x
11.0
x=np.mean(runs[9])
x
84.0
x=np.mean(runs[10])
x
50

Q4]
import numpy as np 
sales_data = np.array([    [150, 200, 250, 300, 400, 350, 500],  [120, 180, 210, 240, 310, 280, 400],    [100, 130, 190, 220, 300, 270, 350],     [80,  90,  150, 180, 240, 220, 300],    [50,  60,  80,  100, 130, 120, 180] ])
1]
y=np.shape(sales_data)
y
o/p:(5,7)
2]
y=np.ndim(sales_data)
y
o/p:2
3]
y=np.dtype(sales_data)
y
nbytes
4]
y=np.size(sales_data)
y
35
5]


