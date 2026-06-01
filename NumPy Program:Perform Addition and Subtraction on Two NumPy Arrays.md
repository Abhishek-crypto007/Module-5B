
# Python Program to Perform Addition and Subtraction on Two NumPy Arrays

## 🎯 Aim
To write a Python program that performs addition and subtraction operations on two NumPy arrays.

## 🧠 Algorithm
1. Import the `numpy` library.  
2. Read two arrays from the user using `eval(input())`.  
3. Convert the inputs into NumPy arrays using `np.array()`.  
4. Perform addition using `arr1 + arr2`.  
5. Perform subtraction using `arr1 - arr2`.  
6. Print the results.  

## 🧾 Program
```python
import os
os.environ["OMP_NUM_THREADS"] = "1"
import numpy as np

arr1 = np.array(eval(input("Enter first array: ")))
arr2 = np.array(eval(input("Enter second array: ")))

print("Addition:\n", arr1 + arr2)
print()
print("Subtraction:\n", arr1 - arr2)
```

## 🖥️ Example Output

<img width="1425" height="915" alt="image" src="https://github.com/user-attachments/assets/f9ae734b-76b7-4a76-a614-ebe79584d9d4" />


## ✅ Result
Thus, the program has been successfully executed to perform addition and subtraction on two NumPy arrays.
