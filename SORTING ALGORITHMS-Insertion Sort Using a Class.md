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
~~~c
class InsertionSorter:
    def __init__(self):
        self.numbers = []
    def input_numbers(self):
        user_input = input("Enter numbers separated by spaces: ")
        try:
            self.numbers = list(map(int, user_input.strip().split()))
        except ValueError:
            print("❌ Please enter valid integers.")
            exit()
    def insertion_sort(self):
        for i in range(1, len(self.numbers)):
            key = self.numbers[i]
            j = i - 1
            while j >= 0 and self.numbers[j] > key:
                self.numbers[j + 1] = self.numbers[j]
                j -= 1
            self.numbers[j + 1] = key
    def display_sorted_list(self):
        print("✅ Sorted list:", self.numbers)
sorter = InsertionSorter()
sorter.input_numbers()
sorter.insertion_sort()
sorter.display_sorted_list()
~~~


## OUTPUT:
![image](https://github.com/user-attachments/assets/e1c97dc7-498d-4646-a310-b766cb7a189a)


## RESULT:
Thus the program has been executed successfully.
