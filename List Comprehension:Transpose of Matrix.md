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
~~~c
class MatrixTranspose:
    def __init__(self, matrix):
        self.matrix = matrix
        self.transposed = self._transpose()
    def _transpose(self):
        return [[self.matrix[row][col] for row in range(len(self.matrix))] 
                for col in range(len(self.matrix[0]))]
    def get_transposed(self):
        return self.transposed
matrix = [
    [1, 2, 3],
    [4, 5, 6]
]

transpose_obj = MatrixTranspose(matrix)
print("Original Matrix:")
for row in matrix:
    print(row)
print("\nTransposed Matrix:")
for row in transpose_obj.get_transposed():
    print(row)
~~~

## OUTPUT:
![Screenshot 2025-05-11 152040](https://github.com/user-attachments/assets/0f78ee12-2589-47cd-9f6a-4d1833e0b597)


## RESULT:
Thus the program has been executed successfully.
