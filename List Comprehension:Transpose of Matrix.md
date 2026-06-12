# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```python
def create(r, c):
    matrix = []
    for i in range(r):
        row = list(map(int, input().split()))
        matrix.append(row)
    return matrix

r = int(input("Enter rows: "))
c = int(input("Enter columns: "))

matrix = create(r, c)

transpose = [[matrix[j][i] for j in range(r)] for i in range(c)]

print("Transpose Matrix:")
for row in transpose:
    print(row)
```

## OUTPUT:
<img width="483" height="300" alt="image" src="https://github.com/user-attachments/assets/13fced62-585c-4996-9396-db81e3fdbe0b" />


## RESULT:
Thus,the program is executed successfully.


