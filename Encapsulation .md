# PYTHON MODULE - 6
# (B) 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM:

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM:

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program:

    class Rectangle:
        def __init__(self):
            self.__length = int(input("Enter a length of the rectangle : "))
            self.__breadth = int(input("Enter a breadth of the rectangle : "))
            self.area = self.__length * self.__breadth
            print(f"Length : {self.__length} sq.units")
            print(f"Breadth : {self.__breadth} sq.units")
            print(f"Area of the Rectangle : {self.area} sq.units")
    call = Rectangle()
    
    # calling the private member outside the class
    print("\nCalling the private members outside the class.....")
    try :
       print("Length of the rectangle : ",call.__length,"sq.units")
    except :
       print("AttributeError: 'Rectangle' object has no attribute '__length'")
    try :
       print("Breadth of the rectangle : ",call.__breadth,"sq.units")
    except :
       print("AttributeError: 'Rectangle' object has no attribute '__breadth'")

## Output:

<img width="1917" height="912" alt="image" src="https://github.com/user-attachments/assets/99828b7a-40be-4e20-926d-91ce91012313" />

## Result:

Thus, The Python program to implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.
 was executed successfully.
