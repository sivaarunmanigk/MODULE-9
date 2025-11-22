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

## 🖥️ Program
~~~c
def read_matrix():
    rows = int(input("Enter number of rows: "))
    cols = int(input("Enter number of columns: "))
    print(f"Enter elements row-wise ({rows} x {cols}):")
    matrix = []
    for i in range(rows):
        row = list(map(int, input(f"Row {i + 1}: ").split()))
        if len(row) != cols:
            print("❌ Invalid number of columns. Please restart.")
            exit()
        matrix.append(row)
    return matrix
def print_diagonals(matrix):
    rows = len(matrix)
    cols = len(matrix[0])
    print("\nDiagonal Elements:")
    for i in range(rows):
        for j in range(cols):
            if i == j:
                print(f"{matrix[i][j]:>4}", end=' ')
            else:
                print("    ", end=' ')
        print()
matrix = read_matrix()
print("\nOriginal Matrix:")
for row in matrix:
    print(row)
print_diagonals(matrix)
~~~

### Output:
![Screenshot 2025-05-11 152358](https://github.com/user-attachments/assets/b01e879a-f8ea-4d57-8917-771888b5cad8)


## Result
Thus the program has been executed successfully.
