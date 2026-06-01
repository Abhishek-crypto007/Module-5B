# 🧪 Pandas Program: Join Two DataFrames Along Columns

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along Columns** (column-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames column-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```python3
import os
os.environ["OMP_NUM_THREADS"]="1"
import pandas as pd
s1=pd.DataFrame(eval(input()))
s2=pd.DataFrame(eval(input()))
print("Original DataFrames:")
print(s1)
print("-------------------------------------")
print(s2)
print()
data=pd.concat([s1,s2],axis=1)
print("Join the said two dataframes along columns:")
print(data)
```

## Output
<img width="1533" height="887" alt="image" src="https://github.com/user-attachments/assets/af483952-650d-43f9-b367-e5ea79289dd4" />

## Result
Thus the is Python program using Pandas to **join two DataFrames along Columns** (column-wise concatenation) and assign all data to a new DataFrame completed successfully.
