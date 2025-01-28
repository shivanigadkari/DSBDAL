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
import numpy as np

# Array 1: 2D array (11x5)
sales_data1 = np.array([
    [45, 50, 30, 60, 25],
    [10, 15, 5, 20, 12],
    [80, 60, 75, 100, 90],
    [25, 30, 20, 35, 40],
    [0, 5, 10, 0, 2],
    [50, 55, 60, 65, 70],
    [35, 40, 45, 50, 55],
    [100, 110, 120, 115, 125],
    [10, 12, 15, 10, 8],
    [70, 80, 85, 90, 95],
    [40, 45, 50, 55, 60]
])

# Array 2: 3D array (2x3x4)
sales_data2 = np.array([[[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]],
                        [[13, 14, 15, 16], [17, 18, 19, 20], [21, 22, 23, 24]]])

# Array 3: 1D array of 100 elements
sales_data3 = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 10)

# Array 4: 2D array (4x5)
sales_data4 = np.array([
    [1, 2, 3, 4, 5],
    [6, 7, 8, 9, 10],
    [11, 12, 13, 14, 15],
    [16, 17, 18, 19, 20]
])

# Array 5: 3D array (2x2x3)
sales_data5 = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])

# Calculate the memory usage for each array
memory_usage1 = sales_data1.nbytes
memory_usage2 = sales_data2.nbytes
memory_usage3 = sales_data3.nbytes
memory_usage4 = sales_data4.nbytes
memory_usage5 = sales_data5.nbytes

# Display the memory usage for each array
print(f"Memory used by sales_data1: {memory_usage1} bytes")
print(f"Memory used by sales_data2: {memory_usage2} bytes")
print(f"Memory used by sales_data3: {memory_usage3} bytes")
print(f"Memory used by sales_data4: {memory_usage4} bytes")
print(f"Memory used by sales_data5: {memory_usage5} bytes")

o/p:
Memory used by sales_data1: 220 bytes
Memory used by sales_data2: 96 bytes
Memory used by sales_data3: 400 bytes
Memory used by sales_data4: 80 bytes
Memory used by sales_data5: 48 bytes

6]
import numpy as np
  sales_data = np.array [45, 50, 30, 60, 25],  # Product 1
    [10, 15, 5, 20, 12],   # Product 2
    [80, 60, 75, 100, 90], # Product 3
    [25, 30, 20, 35, 40],  # Product 4
    [0, 5, 10, 0, 2]       # Product 5
])

product_3_day_4 = sales_data[2, 3]

all_sales_product_1 = sales_data[0, :]

last_2_days_sales = sales_data[:, -2:]

print(f"Sales data for Product 3 on Day 4: {product_3_day_4}")
print(f"All sales data for Product 1: {all_sales_product_1}")
print(f"Sales data for the last 2 days:\n{last_2_days_sales}")

O/P:
Sales data for Product 3 on Day 4: 100
All sales data for Product 1: [45 50 30 60 25]
Sales data for the last 2 days:
[[ 60  25]
 [ 20  12]
 [100  90]
 [ 35  40]
 [  0   2]

 7]
 import numpy as np
sales_data = np.array([
    [45, 50, 30, 60, 25],  # Product 1
    [10, 15, 5, 20, 12],   # Product 2
    [80, 60, 75, 100, 90], # Product 3
    [25, 30, 20, 35, 40],  # Product 4
    [0, 5, 10, 0, 2]       # Product 5
])
first_3_products_sales = sales_data[:3, :]
last_2_days_sales = sales_data[:, -2:]

print("Sales data for the first 3 products:")
print(first_3_products_sales)

print("\nSales data for the last 2 days:")
print(last_2_days_sales)

O/P:
Sales data for the first 3 products:
[[ 45  50  30  60  25]
 [ 10  15   5  20  12]
 [ 80  60  75 100  90]]

Sales data for the last 2 days:
[[ 60  25]
 [ 20  12]
 [100  90]
 [ 35  40]
 [  0   2]]

 8]
# Transpose the array so that rows represent days and columns represent products
transposed_sales_data = sales_data.T

# Display the transposed arraY
print("Transposed sales data (Days as rows, Products as columns):")
print(transposed_sales_data)

O/P:
Transposed sales data (Days as rows, Products as columns):
[[ 45  10  80  25   0]
 [ 50  15  60  30   5]
 [ 30   5  75  20  10]
 [ 60  20 100  35   0]
 [ 25  12  90  40   2]]

