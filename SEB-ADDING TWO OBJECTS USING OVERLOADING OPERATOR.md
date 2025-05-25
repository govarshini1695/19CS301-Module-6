SEB-ADDING TWO OBJECTS USING OVERLOADING OPERATOR

AIM:
TO write a python program using the overloading operator for adding two objects.

ALGORITHM:
   STEP 1:Start the program
   STEP 2:Define a class with appropriate attributes.
   STEP 3:Create a member function to overload the + operator.
   STEP 4:Implement the function to add corresponding attributes of two objects.
   STEP 5:Return a new object containing the sum of attributes. 
   STEP 6:Test the class with appropriate object addition.
   STEP 7:End the program.

PROGRAM:
 
```
class Accessories:
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


![image](https://github.com/user-attachments/assets/0304b366-68ee-4a53-b851-6bd3f4423e90)



RESULT:

Thus the python program using the overloading operator for adding two objects is executed successfully.




