# Python Documentation
## By Noor Raihan

## Chapter 1 : Installation

### Windows Version
1. Visit https://www.python.org/downloads/ and choose which version are suitable. In this case,  we are using Python3 since it have the latest update.
2. After finish the downloading, run the executable Installer and make sure to **tick on *Add Python 3.x to the path***


![[Pasted image 20220410133556.png]]

3. Verify if the Python is successfully installed.
	- Open the command prompt.
	- Type 'python' and press enter.
	- The output should be like this if the python is successfully installed.
	![[Pasted image 20220410133842.png]]

4. Verify if pip is executable through the python command.
	- Open the command prompt.
	- Type this command in the command prompt and press enter.
	```
	python -m pip -V
	```
	- If the installation successfull, you may see the pip version displayed as below.
	![[Pasted image 20220410134406.png]]

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

