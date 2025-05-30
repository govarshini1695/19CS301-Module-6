# 19CS301-Module-6
EX: 6.1   POLYMORPHISM

### AIM: To Create two specific classes- Beans and Mango. Along with that, create a generic function that tells us the type and color of the object we pass. Mind you, since we have passed only “obj” through it, this obj can be any object.

### ALGORITHM:
Step1: create class Beans and def a function type and color

Step 2: create a class Mango and def a function type and color

Step3: def a function func

Step 4: call the objects and execute the program

### PROGRAM:
```
class Beans ():
    def type(self):   
          print("Vegetable")
    def color(self):
          print("Green")
class Mango:
   def type(self):
          print("Fruit")
   def color(self):
         print("Yellow")
   def func(obj):
         obj.type()
         obj.color()
         obj_beans = Beans()
         obj_mango = Mango()
         func(obj_beans)
         func(obj_mango)
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/b41a3e12-896b-4f6c-a9b2-19045a5088f9)


### RESULT: Thus, the program has been successfully executed.

EXP.No: 6.b OPERATOR OVERLOADING

### AIM: write a python program to overload less than operator
###ALGORITHM:
Step1 :create class A and def init	 

Step2: def it	with a condition if self.a < o.a 

Step 3: call the function and execute the program.
### PROGRAM:
```
class A :
     def     init (self,a):
             self.a=a
     def     lt (self,o):
              if self.a < o.a :
                   return "ob1 is less than ob2"
              else:
                   return "ob2 is less than ob1"
ob1 = A(2)
ob2 = A(3)
print(ob1<ob2)
```
###OUTPUT:
![image](https://github.com/user-attachments/assets/dae03d17-1004-424e-a179-ef62fd2681bd)



###RESULT: Thus, the program has been successfully executed.
EX: 6.3 ABSTRACT CLASS METHOD

### AIM: To Create the abstract method calculate_area which is of the abstract class 'Shape'

### ALGORITHM:
Step1:Import ABC and abstractmethod from the abc module.
Step2:Make type_shape inherit from ABC.
Step3:Define an abstract method area using the @abstractmethod decorator.
Step4:Rectangle: Accepts length and width as attributes, implements area().
Step5:Square: Accepts side, implements area().
Step6:Create instances of each subclass and pass appropriate values.
Step7:Call the area method for each object and print the results.

### PROGRAM:
```
from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass

class Rectangle(Shape):
  length = 6
  breadth = 4
  def calculate_area(self):
      return self.length * self.breadth

class Circle(Shape):
  radius = 7
  def calculate_area(self):
      return 3.14 * self.radius * self.radius


class Square(Shape):
  length = 4
  def calculate_area(self):
      return self.length * self.length

class triangle(Shape):
  length = 5
  width = 4
  def calculate_area(self):
      return 1/2 * self.length * self.width
r = Rectangle()
c = Circle()
s = Square() 
t = triangle()
r.calculate_area()
c.calculate_area()
s.calculate_area()
t.calculate_area()
print("Area of a rectangle:", r.calculate_area()) 
print("Area of a circle:", c.calculate_area()) 
print("Area of a square:", s.calculate_area()) 
print("Area of a triangle:", t.calculate_area()) 

```
### OUTPUT:

![image](https://github.com/user-attachments/assets/fb94d2c8-7e21-4156-9dae-e6e49a2ca8c6)


### RESULT: Thus, the program has been successfully executed.

EXP.No: 6.4     ENCAPSULATION

### AIM: To Implement Encapsulation using private members initialized with the value as 22 change the value of the private member using getter and setter methods and also display the value of the version variable.

###ALGORITHM: 
Step1:Create a private member __version initialized to 22.
Step2:Define a method to return the current value of __version.
Step3:Define a method to update the value of __version.
Step4:Call the getter method to display the initial value.
Step5:Change __version to 23 and display the new value.
Step6:Terminate the program.


###PROGRAM:
```
class Robot(object):
    def __init__(self):
       self.__version = 22
    def getVersion(self):
        print(self.__version)
    def setVersion(self, version):
       self.__version=version
obj = Robot()
obj.getVersion()
obj.setVersion(23)
obj.getVersion()

```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/0a7c5af7-e853-4d2c-a0ee-6e8209f5ac26)


### RESULT: Thus, the program has been successfully executed


SEB-ADDING TWO OBJECTS USING OVERLOADING OPERATOR

AIM: TO write a python program using the overloading operator for adding two objects.

ALGORITHM: STEP 1:Start the program STEP 2:Define a class with appropriate attributes. STEP 3:Create a member function to overload the + operator. STEP 4:Implement the function to add corresponding attributes of two objects. STEP 5:Return a new object containing the sum of attributes. STEP 6:Test the class with appropriate object addition. STEP 7:End the program.

PROGRAM:

```class Accessories:
    def __init__(self,a,b):
        self.a=a
        self.b=b
    def __mul__(self,z):
        return self.a+z.a,self.b+z.b
        
a=int(input())
b=int(input())
print("apple and mango mixed:" ,a+b)
c=str(input())
d=str(input())
print("fruit mix: " ,c+d)
```

OUTPUT:

RESULT:

Thus the python program using the overloading operator for adding two objects is executed successfully.

