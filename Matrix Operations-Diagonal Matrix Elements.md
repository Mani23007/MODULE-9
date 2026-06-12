# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program:
```python
r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

matrix = []

for i in range(r):
    row = list(map(int, input().split()))
    matrix.append(row)

print("Matrix:")
for row in matrix:
    print(row)

print("Diagonal Elements:")
for i in range(r):
    for j in range(c):
        if i == j:
            print(matrix[i][j], end=" ")
        else:
            print(" ", end=" ")
    print()
```
### Output:
<img width="489" height="425" alt="image" src="https://github.com/user-attachments/assets/20bc3f0d-9df5-4d02-87ed-3421e2246543" />


## Result:
Thus, the program is executed successfully.
