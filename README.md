git clone <Exercise3>
# Lambda expression to multiply two numbers
product = lambda x, y: x * y

# Test
print("1. Lambda product test:")
print(product(5, 6))  


# Import math module
import math

# Function to calculate the area of a circle
def circle_area(radius):
    return math.pi * radius ** 2

# Test
print("\n2. Area of circle test:")
print(circle_area(10))  

# Function to perform arithmetic operations
def calculator(a, b, operation):
    if operation == 'a':  
        return a + b
    elif operation == 's':  
        return a - b
    elif operation == 'm':  
        return a * b
    elif operation == 'd':  
        return a / b
    else:
        return "Invalid operation"

# Test
print("\n3. Calculator test:")
print(calculator(2, 5, 'd'))  

# Rectangle class
class Rectangle:
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def area(self):
        return self.length * self.width

# Test
print("\n4. Rectangle area test:")
r = Rectangle(5, 10)
print(r.area())  


# Shape base class
class Shape:
    def __init__(self, name, length):
        self.name = name
        self.length = length

    def area(self):
        return 0

# Square subclass
class Square(Shape):
    def __init__(self, name, length):
        super().__init__(name, length)

    def area(self):
        return self.length ** 2

    def describe(self):
        return f"This is a: {self.name}"

# Test
print("\n5. Square class test:")
s = Square('square', 5)
print("The area is:")
print(s.area())       
print(s.describe())   

