# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
~~~c
class EvenNumberGenerator:
    def __init__(self, start, end):
        self.start = start
        self.end = end
        self.even_numbers = self._generate_even_numbers()
    def _generate_even_numbers(self):
        return [num for num in range(self.start, self.end + 1) if num % 2 == 0]
    def get_even_numbers(self):
        return self.even_numbers
generator = EvenNumberGenerator(200, 300)
print(generator.get_even_numbers())
~~~

## OUTPUT:
![Screenshot 2025-05-11 151812](https://github.com/user-attachments/assets/6b39eeff-1859-4d76-88e6-2edf754dca88)


## RESULT:
Thus the program has been executed successfully.
