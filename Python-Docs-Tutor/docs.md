# Python Documentation
## By Noor Raihan

## Chapter 1 : Installation

### Windows Version
1. Visit https://www.python.org/downloads/ and choose which version are suitable. In this case,  we are using Python3 since it have the latest update.
2. After finish the downloading, run the executable Installer and make sure to **tick on *Add Python 3.x to the path***


![[img1.png]]

3. Verify if the Python is successfully installed.
	- Open the command prompt.
	- Type 'python' and press enter.
	- The output should be like this if the python is successfully installed.
	![[img2.png]]

4. Verify if pip is executable through the python command.
	- Open the command prompt.
	- Type this command in the command prompt and press enter.
	```
	python -m pip -V
	```
	- If the installation successfull, you may see the pip version displayed as below.
	![[img3.png]]

5. Now you have successfully install python in your windows machine.


###  Ubuntu version
1. Open the terminal.
2. Enter the command below in the terminal.
	```
	sudo apt install python3
	```
3. Enter 'python' in the terminal.
4. Your're done.








## Chapter 2 : Basic Syntax
####  1. Executing Python program
All python programs and files are ended with **.py** as file extension. It can be executed by using the terminal or command prompt. Both are using the same concept and same command.

You can try create a file called **hello.py** and type this code in the file.
```python
print("Hello world")
```

After that, type the following command in the terminal and make sure the terminal directory are in the same file as the python file.
```
python hello.py or python3 hello.py
```
![[pytest.png]]

#### 2. Printing and displaying text
All programming language start with displaying **Hello World**. In Python3, displaying text are very simple.

```python
print("Hello World!")
```


#### 3. Comments for life
Commenting are very important in explaining what's goin on with our code. It will make the code more readable.

This is how we comment in python3
```python
#This is the comment
```

```python
#This code display hello world
print("hello world")
```

```python
#This is how
#we multiline
#comment
```


#### 4. Variablesssssss
Declaring variable in python are quite simple. You do not need to declare any particular data type and even change the same variable with another datatype.

```python
number = 7 #data type is int
number = "seven" #data type is string now
```

You can display the variable using print right away.

```python
number = 7
print(number)
```

You can display multiple variable too.

```python
x = "This is"
y = "number"
num = 7
print(x, y, num)
```

Print the length of the string

```python
x = "Hello"
print(len(x)) #output would be 5
```

Access every letter in string

```python
x = "hello"
print(x[0]) #output would be "h"
```

If you really want to set the data type, you can use casting on it.

```python
number = str(7) #now it "7"
number = int(7) #now it 7
number = float(7) #now it 7.0
```


#### 5.Playing with numbers and operators

Check which number is minimum
```python
print(min(4,7)) #output would be 4
```

Check which number is maximum
```python
print(max(4,7)) #output would be 7
```

Round up the decimal
```python
print(round(3.5)) #output would be 4
```

Using operater in python
```python
x = 3
y = 6

print(x + y) #output 9
print(x - y) #output -1
print(y / x) #output 2.0
print(y % x) #output 0

```

#### 6. Conditional If..Else
In conditional statement in python, indention are very important and wrong indention can return to syntax error.

If statement
```python
a = 20
b = 150

if b > a:
	print("b is larger than a")

b is larger than a
```

elif statement
```python
a = 20
b = 20

if b > a:
	print("b is larger than a")
elif b == a:
	print("b is equal to a")

#output would be "b is equal to a"
```

else statement
```python
a = 200
b = 50

if b > a:
	print("b is larger than a")
elif b == a:
	print("b is equal to a")
else
	print("a is larger than b")

#output would be "a is larger than b"
```

And statement (both condition must return true)
```python
a = 200  
b = 33  
c = 500 

if a > b and c > a:  
	print("Both conditions are True")
```

Or statement
```python
a = 200  
b = 33  
c = 500  

if a > b or a > c:  
	 print("At least one of the conditions is True")
```

Nested if
```python
x = 41  
  
if x > 10:  
	 print("Above ten,")  
	 if x > 20:  
		 print("and also above 20!")  
	 else:  
		 print("but not above 20.")
```

Pass statement (used when there is nothing to put in if statement and wanted to avoid any error)

```python
a = 33  
b = 200  
  
if b > a:  
	 pass
```

#### 7. User input
User input is very important in every programming language. This is how we receive user input in python3. 
**Remind: input in python always return as string**

```python
name = input("What is your name: ")
print("Your name is", name)
```

#### 8. Loop
There is two type of loops in python.
- **while** loops
- **for** loops

##### While Loop
while loops is a loops that can execute as long as the condition is **true**.
```python
i = 1 #declare the counter

while i < 6: #condition for while loop
	print(i)
	i += 1 #update the counter
```

break statement (it will stop the loop if the condition is true)
```python
i = 1

while i < 6:
	print(i)
	
	if i == 3: #if i is equal to 3 then the loop will stop immediately
		break
		
	i += 1
```

continue statement (it will stop the currect loop status and continue to the next loop)
```python
i = 0

while i < 6:

	i += 1
	if i == 3: #if i is equal to 3 then it will continue to next loop
		continue
		
	print(i)
```

##### For loops

for loop is used to iterate over sequence such as list and arrays
```python
cars = ["Proton", "Honda", "Toyota"]

for x in cars:
	print(x)
```

interestingly it also can be used to iterate through string
```python
for x in "proton":
	print(x)
```

break statement also can be used in for loops
```python
cars = ["Proton", "Honda", "Toyota"]

for x in cars:
	print(x)
	if x == "Honda":
		break
```

same goes to the continue statement
```python
cars = ["Proton", "Honda", "Toyota"]

for x in cars:
	if x == "Honda":
		continue
	print(x)
```

if we have our own counter and range, we can use **range()** in for loops as counter
```python
#it will loop 6 times
for x in range(6):
	print(x)
```

we also can put starting point using range ( range(start, end) )
```python
for x in range(2, 6):
	print(x) #2,3,4,5
```


#### Function
Function can be implemented in python by using **def** (definition)
```python
def hello():
	print("hello")

hello() #output is "hello"

```

def in python also can received any parameter
```python
def hello(text):
	print(text)

hello("hello")

```

or return anything
```python
def hello():
	return "hello"

print(hello()) #output is "hello"

```

```python
def isTrue():
	return True

print(isTrue()) #output is True

```
