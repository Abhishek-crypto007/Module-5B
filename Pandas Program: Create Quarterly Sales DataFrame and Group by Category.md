
# Python Program to Create Quarterly Sales DataFrame and Group by Category

## 🎯 Aim
To write a Python program that creates a DataFrame of quarterly sales, where each row contains the item category, item name, and expenditure. Then group the rows by category and print the total expenditure per category.

## 🧠 Algorithm
1. Import the `pandas` library.  
2. Read the sales data and column names from the user.  
3. Create a DataFrame using `pd.DataFrame(data, columns=col)`.  
4. Group the DataFrame by the `itemcat` column using `.groupby()`.  
5. Compute the sum of expenditures for each category using `.sum()`.  
6. Print the original DataFrame and the grouped result.  

## 🧾 Program
```python
import os
os.environ["OMP_NUM_THREADS"] = "1"
import pandas as pd

data = eval(input("Enter sales data: "))
col = eval(input("Enter column names: "))

qrtsales = pd.DataFrame(data, columns=col)
print(qrtsales)

qs = qrtsales.groupby('itemcat')
print("Result after Filtering Dataframe")
print(qs['expenditure'].sum())
```

## 🖥️ Example Output
<img width="1529" height="906" alt="image" src="https://github.com/user-attachments/assets/8fbc60ac-b564-4577-babd-9b733236515f" />



## ✅ Result
Thus, the program has been successfully executed to create a quarterly sales DataFrame and group the rows by category to calculate total expenditure.
