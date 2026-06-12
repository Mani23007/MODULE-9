# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:
```python
class InsertionSorter:
    def create_list(self):
        n = int(input("Enter number of elements: "))
        self.arr = []

        for i in range(n):
            self.arr.append(int(input()))

    def insertion_sort(self):
        for i in range(1, len(self.arr)):
            key = self.arr[i]
            j = i - 1

            while j >= 0 and self.arr[j] > key:
                self.arr[j + 1] = self.arr[j]
                j -= 1

            self.arr[j + 1] = key

    def print_list(self):
        print("Sorted List:", self.arr)

obj = InsertionSorter()
obj.create_list()
obj.insertion_sort()
obj.print_list()
```
## OUTPUT:
<img width="470" height="279" alt="image" src="https://github.com/user-attachments/assets/569620c9-a350-4bea-8da7-ae3e6b600393" />

## RESULT:
Thus,the program is executed successfully.
