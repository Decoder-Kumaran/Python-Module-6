# PYTHON MODULE - 6
# (A) 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM:

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM:

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program:

    from abc import ABC,abstractmethod
    class Shape:
        @abstractmethod
        def calculate_area(self):
            pass
    class Rectangle:
        def calculate_area(self):
            print("Program to find area of rectangle is executing.....")
            self.length = int(input("Enter The Length Of The Rectangle : "))
            self.breadth = int(input("Enter The Breadth Of The Rectangle : "))
            self.area = self.length*self.breadth
            print(f"Area of The Rectangle is {self.area:.2f} sq.units")
    class Circle:
        def calculate_area(self):
            print("\nProgram to find area of circle is executing.....")
            self.radius = int(input("Enter The Radius Of The Circle : "))
            self.area = 3.14*self.radius*self.radius
            print(f"Area of The Circle is {self.area:.2f} sq.units")
    rec = Rectangle()
    rec.calculate_area()
    cir = Circle()
    cir.calculate_area()

## Output:

<img width="1918" height="912" alt="image" src="https://github.com/user-attachments/assets/cc7c4668-a49f-44f6-be72-6d76b37687aa" />

## Result:

Thus, The Python program to create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle` was executed successfully.
