# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```pyhton
def create_matrix(r, c):
    matrix = []
    for i in range(r):
        row = list(map(int, input().split()))
        matrix.append(row)
    return matrix

r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

print("Enter Matrix A:")
A = create_matrix(r, c)

print("Enter Matrix B:")
B = create_matrix(r, c)

C = []

for i in range(r):
    row = []
    for j in range(c):
        row.append(A[i][j] - B[i][j])
    C.append(row)

print("Resultant Matrix:")
for row in C:
    print(row)
```


## OUTPUT:
<img width="488" height="385" alt="image" src="https://github.com/user-attachments/assets/76b4aa15-ddf0-407f-bd67-2736273f5a56" />


## RESULT:
Thus,the program is executed successfully.

