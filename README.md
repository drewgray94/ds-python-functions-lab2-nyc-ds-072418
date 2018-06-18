
## Basic calculator program using Python

### SWABT

* Combine and experiment with methods taught upto this point including:
        1. Data types 
        2. Iteration 
        3. Conditionals 
        4. Functions 
        5. USER I/O. 

>**EXERCISE: Create a simple calculator which can perform basic arithmetic operations like addition, subtraction, multiplication or division depending upon the user input**.

### Approach 

* User choose the desired operation. Options 1, 2, 3, 4 are valid options for operations.  
* Two numbers are taken and an if…elif…else branching is used to execute a particular section.
* Using functions add(), subtract(), multiply() and divide() evaluate respective operations.

### Example Interface

```
Please select an operation:
1. Add
2. Subtract
3. Multiply
4. Divide

Select operations form 1, 2, 3, 4 : 1
Enter first number : 20
Enter second number : 13
20 + 13 = 33
```

We shall create four functions, one for each arithmatic operation which will perform the required operation and resturn the resulting value as shown below:


```python
Function to add two numbers 
def add(num1, num2):
    return None # Return addition
```

Function to subtract two numbers 

```python

def subtract(num1, num2):
    return None # Return subtraction
```

Function to multiply two numbers
```python

def multiply(num1, num2):
    return None # Return Product
```

Function to divide two numbers
```python

def divide(num1, num2):
    return None # Return Division
```

The main program body to take user input and call the relevent function

Print user menu 
```python

print("Please select operation -\n" \
        "1. Add\n" \
        "2. Subtract\n" \
        "3. Multiply\n" \
        "4. Divide\n")

select = None
 
number_1 = None
number_2 = None

#Use a series of if-elif-else commands to pass the number to desired function defined above

  
DESIRED OUTPUT: 

```

    Please select operation -
    1. Add
    2. Subtract
    3. Multiply
    4. Divide
    
    Select operations form 1, 2, 3, 4 :3
    Enter first number: 3
    Enter second number: 3
    3 * 3 = 9


We can see how the logic set by using if-else statements, along with functions can be used to control the flow of the program in an easy way. Let's add more functionality to our calculator as below:

>Lets try to make it a bit more interesting by introducing the behaviour of a real calculator so our users can choose to either continue with calculationa OR exit the system. Users gets this functionality by pressing `y` for yes and `n` for no towards continuation.

### Example Interface

Notice `continue: y/n` at the bottom of interface.

```
Please select an operation:
1. Add
2. Subtract
3. Multiply
4. Divide

Select operations form 1, 2, 3, 4 : 1
Enter first number : 20
Enter second number : 13
20 + 13 = 33

**Continue: y/n**
```
Write the code below to achieve this functionality

```python
#initialize the code with cont (continue) flag set to yes (y)
cont = 'y'

#Check for user input after each iteration of the code
#Repeat the code above as long as cont = y 
#Break out of code if cont = n (Hint: use a while loop)

#Expected output 

#Select operations form 1, 2, 3, 4 :3
#Enter first number: 2
#Enter second number: 4
#2 * 4 = 8
#Continue? y/n:y
#Select operations form 1, 2, 3, 4 :2
#Enter first number: 4
#Enter second number: 5
#4 - 5 = -1
#Continue? y/n:n

```

The while loop shown above allows the iteration through the code until a specific input from user i.e. `n` is noticed. Let's add some more functionality to this code by asking users about the type of division they are interested in, and this could be either normal division (as before) or a modulo operator (shows remainder).

> Exercise: Change the code in the division function so that if a user selects division operation, the code should ask the user if he/she wants a normal division `/` (int) or `//` (float) , or a module `%` operator which only returns the remainder of a division. The program should return an exception for any other inputs. 


```python
#Redefine the division function including modulo and integer division

def divide(num1, num2):

    # Add a condition to existing function which prompts user for selecting division vs. modulo.
    
#Expected Output: 

#Select operations form 1, 2, 3, 4 :4
#Enter first number: 5
#Enter second number: 4
#Press d for division and m for modulo operator: m
#5 / 4 = 1
#Continue? y/n:y
#Select operations form 1, 2, 3, 4 :4
#Enter first number: 5
#Enter second number: 4
#Press d for division and m for modulo operatord: d
#5 / 4 = 1.25
#Continue? y/n:

```

### Summary

In this lab we saw how loops and conditions can be used to control the logic of a program execution based on user input. We started with building a simple calculator and incrementaly added more functionality to it by adding loops for iteration and further conditions allowing different type of calculations. We also practiced User I/O by taking choices from the users and dealing with exceptions (unexpected input). 

