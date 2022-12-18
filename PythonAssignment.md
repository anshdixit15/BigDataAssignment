## Assignment Part-1

Q1. Why do we call Python as a general purpose and high-level programming language?
Answer - 
Python is developed and designed to use for wide range of solutions. We can use Python to develope websites, web 
applications and desktop and mobile GUI applications. Also it's free, opensource plateform independent language.
High level language means which can be written and understood by human end, on that criteria Python is not only 
high level language, but one of the most easy language for beginners to learn and apply for effective solutions.

Q2. Why is Python called a dynamically typed language?
Answer - 
We don't need to declare data type of any variable in Python before assigning it which makes it 'Dynamically typed language'.
Python directly stores variable data to memory and while running code it determine what kind of data types are they. This provision
empowers Python programmers to redeclare same variable to different data type.
like - 
x = 30               # is 'int' data type
print(x, type(x))
x = 'hello world'    # which is 'str' data type, without any error.
print(x, type(x))

Q3. List some pros and cons of Python programming language?
Answer - 
Every programming language has its advantage and disadvantage, so has Python. Here are some to notice -
PROS ----
1.- [Easiness ] - Python is easy to learn, we can easily read, and write codes. It provides us provision of sort and effective syntaxes.
     We don't need to put semo-colon at the end of syntax to separate line of codes, we can directly change the line. Loops 
     and conditional statements can be without paranthesis and curlibracket open and straight. Codes are also simple to read and understandable
     in Python.
2.- [Interpreted Execution] - Codes are executed line-by-line which makes Python Interpreted language, so it gives error when it stumble upon
     and stopes and reports the error. Programe can contain multi error but it reports one at a time which makes debugging easy.
3.- [Dynamically Typed] - Python provides system where we don't need to declare variable type before assigning it, which makes it unique from
     other languages and makes it easy to not worry for programmer to data type of vaible to reuse the same variable.
4.- [Libraries to use] - Python got huge numbers of library to support programmers with whole variety of functions. The number is over 350,000 packages,
     which can be very helpful for users.
5.- [Open-source ] - Python is open-source and free to use. We can download the source code for free.

CONS ----
1.- [Memory inefficient] - Python uses much memory, because it takes memory slots and doesn't execuse it until finishing executing programmes.
2.- [Runtime Error] - Runtime error is a drawback of the language due to 'Dynamic typed' nature holding data in variable. A variable holding
     string type of data may hold integer type of data later, which can lead to Runtime Error.
3.- [Lacking Mobile computing] - This is can be one of the biggest disadvatage of Python due to not being supported by Android and iOS as official
     programming language. Although it can be used for mobile purposes but with additional arrangements and efforts. 
Those are the some pros & cons of the language.

Q4. In what all domains can we use Python?
Answer - 

Q5. What are variable and how can we declare them?
Answer - 
In Python, variable is a container that stores values. It doesn't have any especial command or keyword to declare a variable.
Declaring a variable - 
x = 20
name = 'Ansh' 
here we are not usinng any command to declare x or name variable but, just assigning them directly.
Rules of declaring any variable -
1.- A variable name must start with a letter or underscore.
2.- A variable name can not start with a number.
3.- A variable is case-sensitive. 'Hello' and 'hello' are different.
4.- A variable can only contain the alphabet, numbers and underscore. Especial symbols like, $, %, @, etc. are not allowed.
5.- Keywords are reserved so they cannot be used for variable names.

Q6. How can we take an input from the user in Python?
Answer - 
We can use input() function to take input in Python.
Like - 
x = input('enter something')
print(x)
It will print the value of x, given by user.

Q7. What is the default datatype of the value that has been taken as an input using input() function?
Answer - 
input() function gives string data type in ouput regardless data given by user. Like -
input(3) & input(hello), both will be in string type.

Q8. What is type casting?
Answer - 
Python has method to convert a variable of certain data type into other data type, is called Type casting.
as - x = 10  # which is int data type
Now we can convert it into float, string data type as well by using some inbuilt functions
z = float(x)
print(type(z))  # it will give float data type
y = string(x) 
print(type(y))  # it will convert into string data type.
=> Type casting can be done automatically by Python or intentionally by programmers, both way.
Like - 
Automatically ---
a, b = 10, 9.0
z = (a+b)
print(z, type(z))  # it wil give 19.0, float
Or
x = input('enter') # it will convert any type into string

Intetionally ---
z = float(a)
print(z, type(z)) # it will give 10.0, float
z = int(b)
print(z, type(z)) # it will give 9, int
          
Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
Answer - 
No we can not take multiple input in input() function directly but, using split() and list comprehension and assigning input() values to different variables.
Like - 
a, b = input('Enter a number').split()  # it will split both values and assign to a and b separately
print('a :', a)
print('b :', b)

Q10. What are keywords?
Answer - 
Keywords are reserved worlds in any programming language to define any programming procedure, initiating any task to do. In Python,
     there are many keywords like - def, class, return, break, continue, if, else, and, or etc.

Q11. Can we use keywords as a variable? Support your answer with reason.
Answer - 
No, we can not use keywords as variable, because they are resureved and not allowed to. The reason behind not allowing keywords to 
use as variable to prevent any kind of exhaution and confusion by compiler and programmers as well.
As, if we write -

class = 10   # class is keyword 
print(class) # it will give syntax error

Now above we can not use class keyword as variable because interpreter will confuse it as class defining. To prevent such thing it will 
give syntax error.
Similarly -

def return(x, y):   # return is keyword but here as function name
     z = x + y
     return z

So, above we use return as function name, but it is reserved word for returning value to callor.
Now interpreter will confuse what to do with return whether to performe codes under function or return value in parameter, and it may cause
big execution problem.
That is why when we use keword as varialbe, will give error that is why not allowed.
                              
Q12. What is indentation? What's the use of indentaion in Python?
Answer - 
In Python indentation is used to put code in block because it doesn't use paranthesis or flower backet to contain them. It is created by space
and we give four alphabet size space or one tab space.
Under class, function, condition, loops etc. we give them to specify bock of codes to execute.
Like - 
def greet():
     print('Hello !')

or

if 5 > 4:
     print('correct')
else:
     print('incorrect')

we can see the print statement is indented by tab space.

Q13. How can we throw some output in Python?
Answer - 
Either we can use 'return' keyword or 'print()' function to get output.
Like - 
x = 10
y = 20
z = x + y
print(z)

or

def add(a,b):
     return a + b

We can get output of addition using either of them.

Q14. What are operators in Python?
Answer - 
We use operators to perform operations on variables or any values. In python ther are well defined operators to do operations as well.
Like - +, -, *, /, //, =, % etc. are operators in Python.
We can divide operators furthor based on their performance, here are they -
1. - Arithmetic operators =>  +, -, *, /, //, **, % 
2. - Assignment operators =>  =,  +=, -=, *=, /= %=, &= |= etc.
3. - Comparison operators =>  ==, !=, >, <, >=, <=
4. - Logic operators =>  and, or, not, 
5. - Bitwise operators =>   &, |, ^, ~, <<, >>

There are - in, not in, is, is not (Membership operators and Identity) as well.   

Q15. What is difference between / and // operators?
Answer - 
/ gives data in float whether number in integer or float
Like - 
x = 10
y = 2
print(x/y) # will give 5.0, in float type despite of 10 is completely divisible by 2

or

x = 5
y = 2
print(x/y) # will give 2.5, in float type, because 5 is not completely divisible by 2, so it will take decimal value

=> In both cases it gave float outcome.

// gives only integer values, whether number is float or not
Like - 
x = 25
y = 2
print(x//y) # will give 12, it will not take decimal after 12 to divide 25 into 12.5

or

x = 20
y = 2
print(x//y) # will give 10, because it gives outcome in integer

=> In Both cases it giave integer value 

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Answer - 
word = 'iNeuron'
print(word*4)

or 

print('iNeuron'*4)

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
Answer -  

def even_or_odd(given_value):
     if given_value % 2 == 0:
          print('Given value is Even')
     else:
          print('Given value is Odd')

Q18. What are boolean operator?
Answer - 
Boolean operator has only tow outcome 'True' and 'False'. If we use any expression which is true it will give True else False.
Like -   
x = 10
y = 5
print(x > y)  # the boolean value will be True
print(x = y)  # the boolean value will be False

=> Here we are printing boolean value using comparison operators

print(x > y and x == 10)  # it will give True boolean value
print(x < y or y == 5)    # it will give True boolean value
print(x < y  or y == x)   # it will give False boolean value

=> Here we are printing boolean value using logical operators

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```
Answer - 
1 or 0 ,                  OUTPUT => 1
0 and 0 ,                 OUtPUT => 0
True and False and True,  OUTPUT => False

Q20. What are conditional statements in Python?
Answer - 
Conditional statements are method put a certain block of codes under any statement, so if statement condition are met the codes will be 
executed. We use 'if' to make conditional statements and if the statement is True the execucation will take place, if False it will not.
Like -  
x = 10
if x > 5:        # <- conditional statement
     print('True')
     
Here if x > 5: is conditional statement, if it happens to be true the block of code under statement will be executed.
If the condition will not be met, will not give any outcome of code under the condition of 'if'.     

Q21. What is use of 'if', 'elif' and 'else' keywords?
Answer - 
'if' is use to specify condition for any bock of code to be executed. Initially we use 'if' for one condition further 'elif' to give 
multiple conditions and 'else' is used to execute the code which is not based on 'if'  or 'elif' condition, controry or not follows the same conditions.
Like -  
whole_num = [0, 1, 2, 3, 4, 5, 6, 7, 8]    # list of Whole numbers

for x in whole_num:
     if x > 0 and x % 2 == 0:
          print(x, ' is even number')
     elif x > 0 and x % 2 != 0:
          print(x, ' is 0dd number')
     else:
          print(x, ' is neither of them')

Above, 'if' is giving condition to execute code when the value of 'x' will be even, 'elif' condition is, the value 'x' must be odd and 'else' is neither of two, so 
if the value of x is not even or odd then 'else' block of code will be executed. 

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Answer - 
age = int(input('Enter your age'))

if age >= 18:
     print('I can vote')
else:
     print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Answer -  
numbers = [12, 75, 150, 180, 145, 525, 50]

even = [x for x in numbers if x%2==0]
first_num = 0
for i in even:
     first_num += i

print(first_num)

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
Answer -  
def greatest_number(num1, num2, num3):
     if (num1 > num2) and (num1 > num3):
          print(num1)
     elif (num2 > num1) and (num2 > num3):
          print(num2)
     elif (num3 > num2) and (num3 > num1):
          print(num3)

greatest_number()  #  <= we can give 3 inputs of numbers and will return greatest value.

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Answer -  
numbers = [12, 75, 150, 180, 145, 525, 50]

for i in numbers:
if i <=150 and i%5==0:
     print(i)
elif i > 500:
     break

Q26. What is a string? How can we declare string in Python?
Answer - 
String in Python is a single character or a collection of multiple characters, so strings are array of character. We use single ('') double ("") or triple (""" """) quote to create strings.
Like -  
a = 'iNeuron',
b = "I am a student"
c = """Let's see how it works"""

# These are strings assigned with variables

Q27. How can we access the string using its index?
Answer - 
name = 'ansh'
print(name[2])     # accessing string by index

# it will give 's' string 
    
Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
Answer - 
print(string[9:])  # will give 'iNeuron' 

Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
Answer - 
print(string[:-8:-1])  # will print 'norueNi'

Q30. Resverse the string given in the above question.
Answer - 
print(string[::-1])    # will reverse entire string

Q31. How can you delete entire string at once?
Answer - 
We can use 'del' keyword to delete entire string 
Like -  
a = 'name'
del a 
print(a)        # entire string is deleted will not give object value

Q32. What is escape sequence?
Answer - 
Escape sefquence is to include special characters in string. To do it we add backslash(\) before character we want to escape.

Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```
Answer - 
print('iNeuron\'s Big Data Course')

Q34. What is a list in Python?
Answer - 
List stores multiple data in single variable. Data can be different types and are changable and accessible in list. List stored items in order and we can access them in 
that order.

Q35. How can you create a list in Python?
Answer - 
We use square bracket to collect all items seperated by comma, and assign them to a variable.
my_list = ['ansh', 1, 5.6, 'dixit', ('iNeuron', 'student')]     # my_list is list containing multiple types of values

Q36. How can we access the elements in a list?
Answer - 
We can access list elements by their order in which they are stored.
my_list = ['ansh', 1, 5.6, 'dixit', ('iNeuron', 'student')]       
print(my_list[0])       # accessing my_list elements by index
print(my_list[3])
        
Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 
Answer - 
print(lst[4][2])       # we can use double indexing to access list inside list

Q38. Take a list as an input from the user and find the length of the list.
Answer -    
def lst_lenght(lst):
    print(len(lst))

lst_lenght(my_lsit)     # it will take input of list and give its length

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```
Answer - 
We use 'insert()' method to add at specific index
lst.insert(3, 'Big')

Q40. What is a tuple? How is it different from list?
Answer - 
Tuple stores ordered and immutable itmes in it. Tuple and list both stores itmes, but major difference between them in list we can mutate items but in tuple we can not modify or mutate items.

Q41. How can you create a tuple in Python?
Answer - 
We use paranthesis () to collect itmes in it and assign to variable.
my_tup = ('ansh', 2, 4, 5.6, 'dixit')

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.
Answer - 
Tuples are immutable so we can not add any new element to tuple directly, but we can create new tuple and concat them.
tup_1 = ('one', 'two', 'three')         # tuple one
tup_1 += ('Ansh',)                      # adding new tuple with existing one
print(tup_1)                            # new tuple containing name will be added in tup_1

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?
Answer - 
We can not append any new element to tuple directly, because tuple is not changable, can not be modified, but we can use type casting method to convert tuple into list and append
new element and reconvert into tuple.
tup_1 = ('one', 'two', 'three')
lst = list(tup_1)               # converting into list
lst.append('four')              # appending new element
tupe_1 = tuple(lst)             # reconverting into tuple

Q44. Take a tuple as an input and print the count of elements in it.
Answer - 
tupe_1 = (1, 2, 3, 2, 4, 5, 4, 6, 7, 8)

def count_tuple_elements(tup, element):
    print(tup.count(element))

count_tuple_elements(tup_1, 4)          # function will take tuple and its element to give its frequency/count

Q45. What are sets in Python?
Answer - 
Set stores multiple items, which are unordered, unchangeable and unindexed. Items in set can be removed and added new. In set duplicate items are not allowed, means we can not add duplicate 
ot items it will only give unique values.

Q46. How can you create a set?
Answer - 
We use curli brackets to collect items and assign to a variable.

my_set = {'one', 'two', 'three', 'ansh', 1, 3, 4, 5.6}
print(my_set)

Q47. Create a set and add "iNeuron" in your set.
Answer - 
my_set = {'one', 'two', 'three', 'ansh', 1, 3, 4, 5.6}
my_set.add('iNeuron')                                   # adding 'iNeuron' in my_set 
print(my_set)

Q48. Try to add multiple values using add() function.
Answer - 
add() method only takes one value at a time, we can not give multiple values.
my_set.add('seven', 'six')              # will not take multiple value like this

Q49. How is update() different from add()?
Answer - 
update() method takes one or multiple iterables in parameters unlike add() which takes one items at a time. update() can take list, tuple or dictionary, it will convert into set and add into 
existing set. Whereas add() takes one value ont multiple iterable argument.  

Q50. What is clear() in sets?
Answer - 
clear() method removes all elements from set give empty set set().
my_set.clear()          # it will remove all elements from my_set  

Q51. What is frozen set?
Answer - 
The frozen set is immutable, unordered, and unique set. Once set is frozen we can not add, remove or update set because it is immutable. We can use frozenset() method to convert into frozen set.

Q52. How is frozen set different from set?
Answer - 
The one base difference is between frozen set and set is, set can be mutated and frozen set can not be mutated. We can not use add(), remove(), update() methods to mutate frozen set unlike
set.

Q53. What is union() in sets? Explain via code.
Answer - 
The union() method creates new set and unify all distinct (unique) values of sets.
A = {1, 3, 5, 3}
B = {9, 7, 6, 5, 7}
C = {'iNeuron', 'ansh', 'iNeuron'}
print(A.union(B, C))       # it will give {1, 3, 5, 6, 7, 9, 'iNeuron', 'ansh'} unique values.

Q54. What is intersection() in sets? Explain via code.
Answer - 
The intersection() method returns a new set with elements that exist or common to all sets.
A = {1, 2, 3}
B = {2, 3, 4, 5}
print(A.intersection(B))        # output will be {2, 3}

Q55. What is dictionary in Python?
Answer - 
Dictionary stores data in key:value form. Data stored in dictionary is ordered and changable but not duplicates are allowed.

Q56. How is dictionary different from all other data structures.
Answer - 
In other data structure there values stored, except sets(elements can't be accessed using index) we access their elements by index. When it comes to dictionary, its data structure is base on keys and values,
and we access and change them by their keys.   

Q57. How can we delare a dictionary in Python?
Answer - 
We can declare dictionary by using curly brackets ans assigning them to variable.
dict_one = {'one':1, 'name':'ansh', 10:'ten'}       # declaring dictionary

Q58. What will the output of the following?
```
var = {}
print(type(var))
```
Answer - 
It will give type class of 'var' <class 'dict'>

Q59. How can we add an element in a dictionary?
Answer - 
We can add element to dictionary using index key and assign to value.
A = {'one':1, 'two':2}
A['tree'] = 3
print(A)

Q60. Create a dictionary and access all the values in that dictionary.
Answer - 
dict_one = {'name':'Ansh', 'student':'iNeuron', 'course':'BigData'}
print(dict_one.values())    # we can use values() method to access all dictionary values.

Q61. Create a nested dictionary and access all the element in the inner dictionary.
Answer - 
nested_dict = {'one':1, 'two':2, 'info':{'name':'Ansh', 'student':'iNeuron', 'course':'BigData'}, 'three':3}
print(nested_dict['info'])      # accessing all elements(key:value) in nested_dict

Q62. What is the use of get() function?
Answer - 
The get function gives value of given key in parameter if exists in dictionary, or it will return 'None'. We can give any message in case the value not found.
dict_one.get('ten', 'Not found')        # it value of key 10 doesn't exest, get() will return 'Not found' message. 

Q63. What is the use of items() function?
Answer - 
The items() will return view object which displays entire key & value of dictionary in tuple pair of key/value.
print(dict_one.items())         # it will return view object of keys/values.

Q64. What is the use of pop() function?
Answer - 
The pop() method removes and return particular element form dictionary.
A = {1:'one', 2:'two', 3:'three'}
print(A.pop(2))         # will remove 2:'two' and give value 'two'
print(A)                # it has only 1 and 3 keys/values.

Q65. What is the use of popitem() function?
Answer - 
The popitem() method removes last added key-value and returns them in tuple.
A = {1:'one', 2:'two', 3:'three'}
print(A.popitem())      # will remove 3:'three' and returns (3, 'three') in tuple form
print(A)                # it has only {1:'one', 2:'two'} key-value.

Q66. What is the use of keys() function?
Answer - 
The keys() method return view object displaying list of all keys.
print(A.keys())         # will give view object displaying list of all keys of A 

Q67. What is the use of values() function?
Answer - 
The values() method return view object containing list of all values of dictionary.
print(A.values())       # will give view object and list of values.

Q68. What are loops in Python?
Answer - 
Loops are a kind of constructs that repeatedly execute a block of code based on certain conditions. In Python we use loop for the same purpose to repeat codes execution.
We firstly write condition and under that conditonal block piece of codes to execute repeatedly untill codes are following the conditions to be true. Loops follow these stpes -
1. - Check condition
2. - If true, execute the block under it.
3. - If false, come out the loop.

Q69. How many type of loop are there in Python?
Answer - 
There are two basic types of loop in Python.
1. While loop
2. For loop 
But baseded on the way of using it, there are three -
While, For & Nested While/For loops.

Q70. What is the difference between for and while loops?
Answer - 
1.- In 'for' loop initialization, conditional checking, and increment/ decrement is done while iteration. In 'While' initialization and condition checking is done first and in body block
increment or decrement is done.
2.- 'For' loop is used when we know the number of iterations at the time of execution. In 'while' loop the number of iteration is unknown.
3.- We do not write direct condition for iteration in 'for' loop like - 
for object in sequence:
    <body>
But in 'while' we write condition to be true to execute body block codes, like - 
while condition:
    <body>

Q71. What is the use of continue statement?
Answer - 
The continue statement is a loop control statement. It forces loop to skip the iteration followed by continue statement and start from next iteration.
for i in range(1,11):
    if i == 5:          # statement for continue
        continue        # using 'continue'
    print(i)            # it will skip print of 5 
    
Q72. What is the use of break statement?
Answer - 
The break statement is used to terminate the execution of loop followed by its conditional statement. We use 'break' inside body of loop under conditional statement to terminate current loop.
for i in range(1,11):
    if i == 7:          # conditional statement of break
        break           # 'break' keyword
    print(i)            # it will terminate iteration when value of 'i' is 7

Q73. What is the use of pass statement?
Answer - 
The pass statement is a null statement, when we don't want to write and implement and code, we just use pass indicate we don't want to execute anything yet but it is placeholder to use this 
place for future. We can use pass statements in class, function or in if-else conditions.
class Demo:         # we created class using pass statement where we don't want to implement any method or attributes.
    pass

def demo:           # we created function using pass statement where we didn't write any codes to execute.
    pass

Q74. What is the use of range() function?
Answer - 
The range() function is used to generate sequence of numbers given in range() function, commanly used to iterate them. The range() function takes three arguments, first where to start, second where to end,
and third steps.
for i in range(1,11,1):     # it will generate numbers 1 to 10 adding 1 steps in it (end number is excluded)
    print(i)

Q75. How can you loop over a dictionary?
Answer - 
Dictionary has two elements, keys and values. We can loop them seperatly not simultaneously, means one by one.
demo_dict = {'name':'Ansh', 'student':'iNeuron', 'course':'BigData'}

for i in demo_dict:         # it will loop keys.  
    print(i)
for i in demo_dict.keys():  # We can use keys() method.
    print(i)

for i in demo_dict:             # it will loop values. 
    print(demo_dict[i])
for i in demo_dict.values():    # We can use values() method for i in demo_dict.values()
    print(i)

### Coding problems
Q76. Write a Python program to find the factorial of a given number.
Answer - 
def factorial(num):
    first_num = 1
    for i in range(1,num+1):
        first_num *= i

    print(first_num)

factorial()            # it will take any number and give factorial

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100
Answer - 
def simple_interest(principal,rate,time):
    si = (principal*rate*time)/100
    print(si)

simple_interest()       # it will give simple interest of principal on certain rate and time.

Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.
Answer - 
def compound_interest(principal, rate, n_years, compound_period=1):
    # four parameters 'principal', 'rate', 'n_years', 'compound_time'
    # 'compound_time' is arbitrary and default to yearly compound time
    # 'compound_time' can be given in fraction or decimal both for half, quarter or monthly like 1/2 or .5
    n_years = n_years / compound_period
    amount = principal* ((1 + ( rate / (100 / compound_period)))**n_years)
    ci = amount - principal
    return ci

compound_interest()     # function compound_interest() will give compound interest

We can give principal money, rate, year and compound period to funtion, it will calculate the compound interest

Q79. Write a Python program to check if a number is prime or not.
Answer - 
def prime_number(number):
    n = number
    if n==2:
        return f'{n} - Prime Number'
    elif (n>1) and (((n % 2 != 0) and (n % 3 != 0 and n % 5 != 0)) or (n / 3 == 1 or n / 5 == 1)):
        return f'{n} - Prime Number'
    else:
        return f'{n} - Not Prime Number'

print(prime_number())       # function prime_number() will check whether number is prime or not

Q80. Write a Python program to check Armstrong Number.
Answer - 
def check_armstrong_number(number):
    str_num = str(number)
    add_power = 0
    for i in str_num:
        power_to = int(i)**len(str_num)
        add_power += power_to
    if add_power==number:
        return f"{number} : Armstrong Number"
    else:
        return f"{number} : Not Armstrong Number"

    # The function check_armstrong_number() will check whether or not a number is Armstrong Number

Q81. Write a Python program to find the n-th Fibonacci Number.
Answer - 
def fibonacci(n):
    # using recursion method to find nth fibonacci number
    if n < 0:
        return 'give positive integer'
    elif n==0:
        return 0
    elif n==1 or n==2:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)

# The function fibonacci() will give nth number of fibonacci number.

Q82. Write a Python program to interchange the first and last element in a list.
Answer - 
def interchange_first_last_el(lst):
    first = lst[0]
    lst[0] = lst[len(lst)-1]
    lst[len(lst)-1] = first
    return lst

    # The function interchange_first_last_el() will interchange the first and last in any list

Q83. Write a Python program to swap two elements in a list.
Answer - 
def swap_elements(lst,index_1, index_2):        
    if index_1 and index_2 <= len(lst-1):
        first_el = lst[index_1]
        lst[index_1] = lst[index_2]
        lst[index_2] = first_el
        print(lst)
    else:
        print('Invalid index : out of list length')
    
    # The function swap_elements() will swap two elements based on given index of elements by user. 

Q84. Write a Python program to find N largest element from a list.
Answer - 
def largest_number(_list):      
    return sorted(_list)[len(_list)-1]
    
# function largest_number() will give largest element form a given list

Q85. Write a Python program to find cumulative sum of a list.
Answer - 
_list = [1,2,3,4,5]
from functools import reduce
sum = lambda x,y:x+y
outcome = reduce(sum,_list)
print(outcome)                  # cumulative sum of _list 

Q86. Write a Python program to check if a string is palindrome or not.
Answer - 
def palindrome_string(word):        
    if word == word[::-1]:
        return f"Yes, The word '{word}' is Palindrome"
    else:
        return f"No, The word '{word}' is not Palindrome"

Q87. Write a Python program to remove i'th element from a string.
Answer - 
def remove_string_element(string, number):
    # Using slicing method to eliminate certain element from string
    # 'number' value can be zero to any integer
    if number > 0:
        rest_string = string[:number] + string[number+1:]
        print(rest_string)
    elif number == 0:
        rest_string = string[1:]
        print(rest_string)
    else:
        rest_string = string[:number-1]
        print(rest_string)

# The function remove_string_element() will remove certain element given from string. 

Q88. Write a Python program to check if a substring is present in a given string.
Answer - 
def check_substring(string, sub_string):
    s_l = string.split()
    if sub_string in s_l:
        return f"Yes! substring '{sub_string}' is present in string"
    else:
        return f"No! substring '{sub_string}' is not present in string"

# Give string and substring in check_substring() function parameter it will check whether it is present or not

Q89. Write a Python program to find words which are greater than given length k.
Answer - 
def greater_length_word(sentence, k):
    word = sentence.split(" ")
    w_l = []
    for i in word:
        if len(i) > k:
            w_l.append(i)
    return w_l

# The function greater_length_word() will give list of words greater than given in parameter 

Q90. Write a Python program to extract unique dictionary values.
Answer - 
demo = {'one': [5,6,7,8,9],
        'two': [1,15,3,20,5,6],
        'three': [9,8,7,6,5],
        'four': [1,15,3,20,5]}

extracted_values = list({dict_el for dict_val in demo.values() for dict_el in dict_val})
print(extracted_values)        
# it will extract unique values of demo dictionary

Q91. Write a Python program to merge two dictionary.
Answer = 
def merge_dict(dict1, dict2):
    return dict1 | dict2

print(merge_dict())     # give input of dictionaries it will merge them

Q92. Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
Answer - 
tuple_list = [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
tuple_to_dict = {a:b for a,b in tuple_list}
print(tuple_to_dict)

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```
Answer - 
list = [9, 5, 6]
tuple_cube_pair = [(a, a**3) for a in list]
print(tuple_cube_pair)

Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
Answer - 
combination_pair = [(x, y) for x in test_tuple1 for y in test_tuple2]
combination_pair += [(x, y) for x  in test_tuple2 for y in test_tuple1]
print(combination_pair)

Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```
Answer - 
def sort_tuple_list(tuple_list):
    for i in range(len(tuple_list)):
        for j in range(len(tuple_list)):
            if tuple_list[j][1] > tuple_list[i][1]:
                tuple_list[j], tuple_list[i] = tuple_list[i],tuple_list[j]

    return tuple_list

# it will sort tuple second values in list

Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
Answer - 
for i in range(5):
    for j in range(i+1):
        print('*', end=" ")
    print()

# It will give the same pattern above mentioned.

Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
Answer - 
rows = 5
s = rows - 1
for i in range(0, rows):
    for j in range(0, s):
        print(end=" ")
    s = s-1
    for j in range(0, i+1):
        print('*', end="")
    print("")

Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
Answer - 
rows = 5
s = rows
for i in range(0, rows):
    for j in range(0, s):
        print(end=" ")
    s = s-1
    for j in range(0, i+1):
        print('* ', end="")
    print("")


Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
Answer - 
rows = 5
for i in range(1, rows+1):
    for j in range(1, i+1):
        print(j, end=" ")
    print()

Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
Answer - 
alpha_value = 65
for i in range(5):
    for j in range(i+1):
        alpha_ch = chr(alpha_value)
        print(alpha_ch, end=" ")
    alpha_value = alpha_value + 1
    print()