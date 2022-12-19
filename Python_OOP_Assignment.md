## Python OOP Assignment

Q1. What is the purpose of Python's OOP?
Answer - 
The basic purporse of OOP in python to solve real world probems creating objects and binding their attribute and behaviour with it.
It also serves purpose of reusibility of codes, we can use the same codes in form of behaviour and attributes given to any objects.
We can restrict access to methods and vairables and this prevents data from direct modification.
By this OOP concept we can programme anything to solve problem and reuse the same code for multiple times. Take example of if we have to 
make a calculator, so we can use this OOP concept to create a blue print of its all attributes and behaviour like add, subtract, division, multiplication
etc. and use its different methods to perform tastk. The great benifit of this thing is that we don't let user to access real methods inside the programmes
and without any modification and knowing about the inside thing they can use the methods.
For python every thing is an object and it has alot of classes as well in different form like str, int, data types and they are all based on the same OOP concept
and we use them without accessing their codes and modifying them, and it makes thing more easy and secure.


Q2. Where does an inheritance search look for an attribute?
Answer - 
There are two kind of class, the first one is parent(base) class and the socond one is child class. The child class inherit attributes from base classes. It can
make attribute of its own but will inherit every attribute from parent class. Every attribute is attached liked tree child to parent class.
So when a child object access attribute it searches like tree bottom to top first in its own class and when it's missing go to parent class. 

Q3. How do you distinguish between a class object and an instance object?
Answer - 
When we create class an object with same name is also created to get class attribute and methods, It is called class object. This attributes and mehtods of class attributes
and methods different from attributes we give throught contructors.  Instance object is when we assign any variable to this class object, it is instance object.
Like - 
class Car:
    
    wheel = 'Four'
    
    @classmethod
    def car_engine():
        print('Diesel and Petrol engine')

    def __init__(self, name, color)
        self.car_name = name
        self.car_color = color

Car.wheel
# 'Car' is class object accessing class attributes and methods                       
Car.car_engine()
car1 = Car('Audi', 'White')     
# 'car1' is instance object assigned to class 'car()' object 

print(car1.car_name)    
# We can accress instance attribute by using instance object, but class object will not work here, because attributes belong to instances
print(Car.wheel)        
# We can access class attribute by using class object, and instance object is assined to class object so it can also access class variable and methods.

Q4. What makes the first argument in a class's method function special?
Answer - 
Class method's first argument is 'cls' refering to class. Likewise 'self' referece of instance object 'cls' refers to class object. We can access class variable through 'cls'.
Like - 
class Employee:
    company = 'Microsoft'

    @classmethod
    def employee_info(cls):   # 'cls' refering to class
        print(cls.company)    # 'cls' accessing class attribute

Employee.employee_info()

Q5. What is the purpose of the __init__ method?
Answer - 
The prupose of __init__ method in Python is to contruct attributes structure of objects, which kind of trait they will have. '__init__' is called constructor
and is inbult method to take arguments which refer to attributes given to objects. Without __init__ method we will not be able to give attributes to objects which variable in nature for 
different objects. If we make any class and define __init__ method and put arguments in for attributes then objects will can assign their specific traits to __init__ arguments and when
it is called, will provide it with objects.
Like - 
class Students:
    def __init__(self, name, age):   # arguments for attributes to assign 
        self.student_name = name     
        self.student_age = age

Now we can make objects and give their attributes (name, age) to them specifically

student_1 = Students('Ansh', 29)

Q6. What is the process for creating a class instance?
Answer - 
If we have class and want to create instance of it, just assign it to any variable name of objct, it will be instance of that class.
Like - 
class Citizen:      # class
    pass

indian = Citizen()   # instance(object) of class

Q7. What is the process for creating a class?
Answer - 
The process of creating class is, first we need to use the keyword 'class' to define class and give name of class putting ':' colon at the end of name. Then we write methods of class under it
either class or instance based on requirements.
Like - 
class Cricket:
    pass

# This is defining Cricket class, now we can give methods to it.

class Cricket:
    test = '5 days'
    oneday = '50 overs'
    t_20 = '20 overs'

    @classmethod
    def game_format(cls):
        return 'Cricket has three format {}, {}, {}'.format(cls.test, cls.oneday, cls.t_20)                

# Here we gave method under class Cricket

Q8. How would you define the superclasses of a class?
Answer - 
Class can inherit attributes and methods of different class. The class class wich is inheriting thing from other class, called 'base'/'child' or 'Subclass', and
the class from which first class inheriting thing, called 'Superclass'. There can be multiple superclassles of a subclass.
Like - 
class Mother:       # superclass
    color = 'Fair'

    @classmethod
    def complexion(cls):
        return cls.color


class Father:       # superclass
    measure = 'Tall'

    @classmethod
    def height(cls):
        return cls.measure


class Kid(Mother, Father):  # subclass (inheriting from superclasses)

    @staticmethod
    def body_feature():
        print("This kid is {} and {}".format(Kid.complexion(), Kid.height()))

# Here 'Mother' and 'Father' are superclasses of a class 'Kid' which is subclass

Q9. What is the relationship between classes and modules?
Answer - 
No direct relationship between classes and modules. Module can be imported and its variables, functions, classes and codes can be resued in different module. It just contains them.
Class is the programming method to create blue print of object and construct its attribute and behaviour. We call different methods on objects to perform its behaviour to give some output.
Though in theory there is no direct relationship between both thing but, they share base trait of reusibility of codes. As above mentioned that module can let us use its containing 
varible, functions and classes features, class also provides the provision of reusability of codes when we call any method on its objects.     
         
Q10. How do you make instances and classes?
Answer - 
We just assign any variable name to class object and can make instances.
Like - 
class Animal:
    pass

dog = Animal()    
# 'dog' is instance assigned to class object Animal

Q11. Where and how should be class attributes created?
Answer - 
Class attributes can be created outside of any function in same block of code with functions. Though it can created anywhere in class but, for better readality we put it top of the codes.
Like - 
class Book:

    message = 'books are good friend of people'    # class attribute at top global reach, readable

    def __init__(self, title):
        self.book_title = title
        print(message)

book_1 = Book('Theory of everything')

print(Book.message)     # can be accessed by class object
print(book_1.message)   # can be accessed by instance object as well

Q12. Where and how are instance attributes created?
Answer - 
Instance attributes are created in constructor __init__ method, we give attribute name in argument form in the parameter.
Like - 
def __init__(self, name, age):    # 'name' and 'age' are instance attribute 
    self._name = name
    self._age = age


Q13. What does the term 'self' in a Python class mean?
Answer - 
'self' is reference of instance object by which we access attributes of perticular object. Without 'self' we will not be able to access individual attributes of 
objects.
Like - 
class Bike:
    def __init__(self, name):
        self.bike_name = name       # 'self' accessing attribute of objects

bike_1 = Bike('R-15')  # object the 'self' refers

Q14. How does a Python class handle operator overloading?
Answer - 
Operator overloading means when a operator behaves differently based on different object. Here is + and * operators they will give different outcome based on 
different data type objects, print(2 + 5) => 7, print('ansh' + 'dixit') => andhdixit, print(2*5) => 10 and print('ansh'*2) => anshansh. 
We can see different outcomes by same operators behaving differently on objects.
Now every data type is class 'str class', 'int class', 'float class' etc. they are all differnt classes and objects are based on theat classes. When we write x = 5
now x's value is 'int' class and if x = 'name' so x's value 'str' class. So when we apply any operator on them the class uses __add__() inbuilt methods to operate
as per defined in class to behave.
Every class data type has its own operator defined to perform as per their requirement, so when we call them on 'int' it will add integers and when we call them on 'str'
it concat the charactors. 
Like - x = ['one', 'four', 'five']
    print(len(x)) => 3  # outcome
    x = 'ansh'
    print(len(x)) => 4  # outcome

# Here we can see the len() function is giving different outcome, in the first it is on list class and the second it is on string class. So both classes are using len()
# function as per their requirements.

Q15. When do you consider allowing operator overloading of your classes?
Answer - 
When i need same method to behave differently for different type of objects, i will consider operator overloading for classes.
Like - 
class Name:
    def __init__(self, first, last):
        self.first_name = first
        self.last_name = last

    def __add__(self. other):
        print(self.first_name + other.last_name)

Q16. What is the most popular form of operator overloading?
Answer - 
Plus operator overloading is most popular operator overloading. It adds numbers and concat string as well,
Like - 
print(10 + 5)   # will add numbers
print('Ansh' + 'Dixit')     # will concat both strings

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?
Answer - 
'Class' and 'Objects' are two main pillar of OOP concept, because OOP is based on objects programming and creating blue prints of objects and creating objects to associate with its
attributes and behaviour is important thing to understand.
Like - 
    class x:    # this is class
        pass

    x1 = x()    # object

# both basic block of OOP concept

Q18. Describe three applications for exception processing.
Answer - 
The applications for exception processing are -
1. - To test any code
2. - To catch any error
3. - To handle that error.

Q19. What happens if you don't do something extra to treat an exception?
Answer - 
If we don't do something extra to reat an exception, the program will crash and interpreter will not execute codes further.

Q20. What are your options for recovering from an exception in your script?
Answer - 
We handle exception using exception keyword and raising error in script, and programme will crash. Under exception block we can write anything to idenfy the exception or error type.
We can use 'finally' keyword as well, because it will execute codes regardless of exception occures or not.

Q21. Describe two methods for triggering exceptions in your script.
Answer - 
### First Method - 
x = 20

try:
    print(x/0)
except ZeroDivisionError as e:
    print(e)
except IndexErro as e:
    print(e)

=> We can write especific error in exception section and print it, but don't know always what kind of exceptin will occure and would need to put multiple exception block like above.
    
### Second Method - 

x = 22

try:
    print(x/0)
except Exception as e:
    print(e)

# This method using 'Exception' keyword will directly evolve the code and identify type of error and give exception, we will not to specify multiple exception blocks

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of
whether or not an exception exists.
Answer - 
#### First Method -

We can use 'finally' keyword after 'exception' it will execute code whether or not exception exitst.
x = 3
try:
    print(x / 0)
except Exception as e:
    print(e)
finally:
    print('The execution is done')

### Second Method - 
We can write code in 'except' block and after use 'else' and put the same code, in this way whether or not exceptin occure it will execute the code
x = 3
try:
    print(x / 0)        # divided by zero
    print(x/2)          # divide by 2 

except Exception as e:
    print(e)
    print("let's see")
else:
    print("let's see")        

# it will print "let's see" regardless the exception

Q23. What is the purpose of the try statement?
Answer - 
The try statement is simply to check if any code has error or not. If code has any error try block will not execute the codes. We chech codes in try block whether they have error or not.
Like - 
x = 10
try:
    print(x/2)

# It will test print(x/2) error 

Q24. What are the two most popular try statement variations?
Answer - 
The two most popular try variations are -
The first is try/except/else and the second is try/except/finally

1. - Try/Except/Else-
We attache else statement after of try/except statement, if no exception occures it will be executed.
try:
    print('Hello')
except Exception as e:
    print(e)
else:
    print('World!')

2. - Try/Except/Finally-
We attache finally statement after of try/except statement, regardless exception occures or not the finally will be executed.
try:
    print(2/0)
except Exception as e:
    print(e)
finally:
    print('This program is closed')

Q25. What is the purpose of the raise statement?
Answer - 
The 'raise' keyword is used to raise any kind of error or exception. 
Like -
try:
    a = 'name'
    num = int(a)
except ValueError:
    raise ValueError('String can not be changed into int')  # it will print message with ValueError error

Q26. What does the assert statement do, and what other statement is it like?
Answer - 
Assert statement in Python to check correctness of codes whether a condtion is true or not. It gives AssertionError when it finds any condition false. It resemles with if and else conditions
like, if staement is true it will execute if block of code either not or else block of codes, or it resemles with try and exception keyword like, if any code has error it will stop execution of 
codes.
Like- 
age = 11
assert age >= 18, f"You are under 18, age {age} is not eligible for casting vote"  

Now above it will raise error AssertionError with message because the condition is not met.

Q27. What is the purpose of the with/as argument, and what other statement is it like?
Answer - 
The purpose of with/as statement is to proper use of external resources in porgrames such as file, lock, network connections etc. It manages resources well by preventing memory leak, and does clean up
actions. If we open any file and use it and forget to close it, so it may be open and would dataloss and memory leak thing happen. with/as statement autometically close the file open in program.
It works like try and finally keyword construct. They also open and without closing close files automatically.
Like - 
with open('text.txt', 'w') as f:        
    f.write('Hello world')
# it will create context manager and directly close file without close programmer

Now we don't need to use f.close statement becuse it will close file automatically when we are done with writing file.
It is like try and finally construct -

file = open('text.txt', 'w')
try:
    file.write("Hello world")
finally:
    file.close()

# It will gurantee close file despite of exception in try block of codes. Same as with statement.


Q28. What are *args, **kwargs?
Answer - 
*args and **kwargs are used to give multiple arguments in function parameter. When we define any function so we give arguments so it will be limited but with use of these special arguments it 
possible to give multiple arguments as required.

*args - It allows to pass varying numbers of positional arguments. The '*' is called unpacking operator will give output in tuple form -
    
def demo(*args):    # *args in parameter
    print(args)

Now we can give any number of arguments it will print them

demo('one', 'two', 'three')     # demo() function will print them all

**kwargs - It accepts multiple keyword arguments. The '**' is unpacking operator will take arguments as dictionary form -

def demo(**kwargs):     # **kwargs in parameter
    print(kwargs)

Now we can give keyword arguments

demo(firstname='ansh', lastname='dixit', student='ineurone')   # will give output in dictionary form

Q29. How can I pass optional or keyword parameters from one function to another?
Answer - 
def demo(*nums, **detail):
    print(nums, detail)

demo(1, 2, 3, 4, 5, name='ansh', project='PythonOOP')   # we are passing optional and keyword arguments to another function while calling it 

Q30. What are Lambda Functions?
Answer - 
A function without name, which is also called anonymous function, is Lambda function. 'lambda' is keyword to define anonymous functions as
'def' is used to define normal functions. It is restricted to one single expression.
Like - 
    add = lambda x,y : x+y  # lambda expression in single expression
    print(add)              # printing function object
                
Q31. Explain Inheritance in Python with an example?
Answer - 
Inheritence is method of programming to achieve the re-usability of codes from other classes. One class can access code form other class. In Python inheritance has the same purpose, to get trait from 
other class to a particular class and re-usability of codes. The class receiving all attributes and methods from, is called 'child/subclass' and, the class
which child class getting things from, is called parent/superclass. We simply add paranthesis next to child class name and put parent class name to inherit traits.
Like - 
class Plant:                                # parent class (superclass)
    def __init__(self, nature):
        self.plant_nature = nature

    def display_plant(self):
        print('Plants', self.plant_nature)


class Flower(Plant):                        # child class (subclass)
    def __init__(self, bud, nature):
        self.flower_bud = bud   
        Plant.__init__(self, nature)    # accessing 'Plant' class attribute

    def display_flower(self):
        print('Flowers', self.plant_nature, 'and', self.flower_bud)     # using 'nature' attribute

plant_1 = Plant('grow')                 # Plant class object
flower_1 = Flower('blossom', 'grow')    # Flower class object

plant_1.display_plant()     

flower_1.display_flower()

# Here we can see class Flower is inheriting attribute and method from Plant class.
# Flower objecst can use Plant method as well.

flower_1.display_plant()
flower_1.display_flower()   # using both class method due to inheritence 

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?
Answer - 
It will invoke class A's func(), because Python uses Method Resolution Order (MRO) to determine to search base class to derive attributes or methods first. In this MRO system base classes are
searched 'Left-to-Right' manner, in our case which is C(A,B), so it will invoke A's func() first.

Q33. Which methods/functions do we use to determine the type of instance and inheritance?
Answer - 
To determine an instance type we use isinstance() function, it tells True or False whether an instance belongs to a particular class or not.
Like - 
a = 10
print(isinstance(a, int))   # it will give True, because 10 belongs to 'int' class

class A:
    pass

a1 = A()
print(isinstance(a1, A))    # it will give True, instance a1 belongs ot A class

So instances are associated with their classes and their types depends on them, when we use 'isinstance()' function it will determine the type of instances.

To determine inheritence type we use issubclass() function, it gives True or False outcome to clarify whether the particular class is child class or not.
Like -
class A:
    pass
class B(A):
    pass
class C(A,B):
    pass

print(issubclass(A, B))         # will give True outcome 
print(issubclass(C, (A,B)))     # will give True 
print(issubclass(A, B))         # will give False

Q34.Explain the use of the 'nonlocal' keyword in Python.
Answer - 
The 'nonlocal' keyword is used to increase scope of access of any variable from enclosed area, which is assigned in inner function of nested functions. Simply when we use nested functions
there is outer function and a inner function in outer function. Now if we want to access a variable assigned in inner function, from outer function section of block, so we can not access 
without using the keyword 'nonlocal', which define the variable can be accessed from outer function block.
Like -
def outer():
    x = 'outer x'
    def inner():
        nonlocal x     # 'nonlocal' keyword to increase access of variable 'x'
        x = 'inner x'
    inner()
    print(x)           # printing (accessing) inner variable x' value

outer()                # it will give 'inner x' outcome

# Here we can see from outer block of code we are printing inner variable value, without 'nonlocal' keyword it will print 'outer x'.

Q35. What is the global keyword?
Answer - 
The 'global' keyword is to let any variable, assigned in a function, to be accesssed outside of function. If we assigned any variable in any function and want to access it from outside of function
we can not access its value without using 'global' keyword to define the variable global to accessed.
Like - 
def demo():
    global x                 # 'global keyword' to define x is global to access
    x = 'hello world !'
    print('from inside -', x)

demo()
print('from outside -', x)   # accessing (printing) from outside of the demo() function 