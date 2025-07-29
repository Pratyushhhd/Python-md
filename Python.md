
# Variable
## string
```
first_name = "Pratyush"
food = "Pizza"
email = "developer.pratyush.787@gmail.com"
print(f"Hello {first_name}")
print(f"You like {food}")
print(f"Your email is {email}")
```
## Integer
``` 
age = 18
quantity = 3
num_of_students = 35

print(f"Your age is {age}")
print(f"You are buing {quantity} items")
print(f"your class has {num_of_students} students ")
```

## Float
```
price = 10.99
gpa = 3.5
distance = 5.5
print(f"The price is {price}")
print(f"Your GPA is {gpa}")
print(f"you ran {distance}km")
```

## Boolean
```

is_student = False
for_sale = True
weather = False
is_online = True
if is_student :
    print("You are a student")
else :
    print("You are not a student")

if for_sale :
    print("This item is for sale")
else:
    print("This item is not for sale")

if is_online :
    print("You are online")
else :
    print('You are offline')
if weather :
    print("It will rain today")
else :
    print("It's not going to rain today")

```

## type casting
```

name = "Pratyush"
age = 18
gpa = 3.5
is_student = True

gpa =int(gpa)
age =str(age)
name =bool(name)

print(name)
print(type(age))
print(type(gpa))
```

## input() = A function that prompts the user to enter data Returns the entered data as a string
```
name = input("What is your name?:")
age = int(input("How old are you?:"))

age = age + 1
print(f"Hello {name}!")
print("Happy Birthday")
print(f"You are {age} years old")

```
# Madlibs game

```

adjective1 = input("enter an adjective (description):")
noun1 = input("Enter a noun ( person, place, thing):")
adjective2 = input("enter an adjective (description):")
verb1 = input("Enter a verb ending with 'ing'")
adjective3 = input("enter an adjective (description):")

print(f"Today I went to {adjective1} zoo.")
print(f"In an exhibit, I saw a {noun1}")
print(f"{noun1} was {adjective2} and {verb1}")
print(f"I was {adjective3}!")

```

# Arithmetic and Math

```

friends = 10

# friends = friends + 1
# friends +=1
# friends = friends-2
# friends-=2
# friends*=3
# friends/=2
# friends **=2
# remainder = friends % 4
# print(remainder)

x = 3.14
y = 4
z = 5

# result = round(x)
# result =abs(y)
# result = pow(4,3)
# result = max(x,y,z)
#result = min(x,y,z)
# print(result)

import math

x = 9.9
# print(math.pi)
# print(math.e)
# result = math.sqrt(x)
# result = math.ceil(x)
result = math.floor(x)
print(result)

```


## Math exercise 1

```
import math

radius = float(input("Enter the radius of a circle:"))

circumference = 2 * math.pi * radius
print(f"The circumference {round(circumference, 2)}")

```

## Math exercise 2

```

import math


radius = float(input("Enter the radius of the circle:"))

area = math.pi * pow(radius, 2)
print(f"The area of the circle is :{round(area, 2)}cm²")

```

## Math exercise 3

```
import math

a = float(input("Enter  side A:"))
b = float(input("Enter  side B:"))

c = math.sqrt(pow(a, 2) + pow(b, 2))
print(f"Side C = {c}")

```

# if_statement


### if = Do some code only If some condition is True
### Else do something else

## Example 1
```
age = int(input("Enter your age:"))

if age >= 89 :
    print("You are too old to sign up")
elif age >= 18:
    print("You are now signed up!")
elif age < 0 :
    print("You have not been born yet")

else:
   print("You must be 18+ to sign up!")

```
## Example 2
 ```
 response = input("Would you like to have some food? (Y/N):")

 if response == "Y" :
      print("Have some food!")
 else:
      print("No food for you!")

```
## Example 3
```
name = input("Enter your name:")
  if name == "" :
     print("You did not type your name!")
 else:
     print(f"Hello {name}")

```
 ## Example 4 (Boolean with if statement)

```
 for_sale = False
 if for_sale :
     print("This item is for sale")
 else:
     print("This item is not for sale")
```

## Example 5


```
online = True
if online :
    print("This user is online")
else:
    print("This user is offline")

```

# Python calculator

```
operator = input("Enter an operator (+ - * /): ")
num1 = float(input("Enter the 1st number:"))
num2 = float(input("Enter the 2nd number:"))


if operator == "+" :
    result = num1 + num2
    print(round(result))
elif operator == "-" :
    result = num1 - num2
    print(round(result))
elif operator == "*" :
    result = num1 * num2
    print(round(result))
elif operator == "/" :
    result = num1 / num2
    print(round(result))
else:
    print(f"{operator} is not a valid operator") 
``` 


# Python weight converter

```

weight =  float(input("Enter your weight:"))
unit = input("Killograms or Pounds(K or L):")
if unit == "K":
    weight  = weight * 2.205
    unit = "Lbs."
    print(f"Your weight is: {round(weight, 1)} {unit}")
elif unit == "L":
    weight = weight / 2.205
    unit = 'Kgs.'
    print(f"Your weight is: {round(weight, 1)} {unit}")
else:
    print(f"{unit} was not valid")

```

# Temperature conversion
```

unit = input("Is this temperature in Celcius or Fahrenheit (C/F):")
temp = float(input("Enter the temperature: "))


if unit == "C" :
    temp = round(9 * temp / 5 +32, 1)
    print(f"The temperature in Fahrenheit is: {temp}°F")
elif unit == "F":
    temp =round((temp - 32) * 5 / 9,1)
    print(f"The temperature in Celcius is: {temp}°C")

else:
    print(f"{unit} is an invalid unit of measurement")

```


# Logical operator

```

# temp = 20
# is_raining = True

# if temp > 35 or temp < 0 or is_raining:
#     print("the outdoor event is cancelled")
# else:
#     print("The outdoor event is still scheduled")

temp = 20
is_sunny = False    

if temp >= 28 and is_sunny:
    print("It is hot outside")
    print("It is sunny")
elif temp <= 0 and is_sunny :
    print("It is cold outside")
    print("it is sunny")
elif 28 > temp > 0 and is_sunny :
    print("It is warm outside")
    print("it is sunny")
elif temp >= 28 and not is_sunny:
        print("It is hot outside")
        print("it is")
elif temp <= 0 and not is_sunny:
        print("It is cold outside")
        print("It is cloudy")
elif 28 > temp > 0 and not is_sunny:
        print("It is warm outside")
        print("It is cloudy")

```

# Conditional operator

```

num = 2
a = 6
b = 7
age = 3
temp = 10
user_role ="guest"
# print("Positive" if num > 0 else "Negative")
# result = "Even" if num % 2 == 0 else "ODD"

max_num = a if a > b else b
min_num = a if a < b else b
status = "Adult" if age >= 18 else "Child"
weather = "Hot " if temp >= 18 else "Cold"
acess_level = "Full Acess" if user_role == "admin" else "limited Acess"


print(acess_level)

```
# String Method 

## Exercise 1
```

name = input("Enter your full name:")
phone_number = input("Enter your phone number")

result = len(name)
result = name.find("r")
result = name.rfind("s")

name = name.capitalize()
name = name.lower()
result = name.isdigit()
result = name.isalpha()
result = phone_number.count("-")
result = phone_number.replace("-", " ")

 print(result)

```
# Exercise 2
```
 username = input("Enter a username: ")


if len(username) > 12 :
    print("Your username can't be more than 12 characters")
elif not username.find(" ") == -1 :
    print("Your username can't contain spaces")
elif not username.isalpha() :
    print("Your username can't contain number")
else:
    print(f"Welcome {username}")

```

### for help print(help(str))

# String indexing

```

# indexing =accesing elements of a sequence using [] (indexing operator)
# [start : end : step]

credit_number = "1234-5678-8939-3456"
credit_number = credit_number[::-1]
last_digit = credit_number [ -4:]


print(credit_number[5])
print(credit_number[0 : 4])
print(credit_number[5 : 9])
print(credit_number[5 : ])
print(credit_number[-1])
print(credit_number[::3])
print(f"XXXX-XXXX-XXXX-{last_digit}")
print(credit_number)

```

# format specifiers
```

# format specifiers = {value : flags} a value based on what flag are inserted

price1 = 3000.14159
price2 = -9870.65
price3 = 1200.34

print(f"price 1 is ${price1:+,.2f}")
print(f"price 2 is ${price2:+,.2f}")
print(f"price 3 is ${price3:+,.2f}")

```

# While loop 

```
# while loop = execute some code WHILE some condition remains true

name = input("Enter your name:")

while name == "" :
    print("You did not enter your name")
    name = input("Enter your name:")
else:
    print(f"Hello {name}")


age = int(input("Enter your age: "))

while age < 0 :
    print("Age can't be negative")
    age = int(input("Enter your age: "))

print(f"You are {age} years old")

food = input("Enter a food you like (q to quit):")

while not food == "q" :
    print(f"You like {food}")
    food = input("Enter a food you like (q to quit):")

print("bye")


num = int(input("Enter a number between 1 - 10:"))

while num < 1 or num > 10:
    print(f"{num} is not valid")
    num = int(input("Enter a number between 1 - 10:"))

print(f"You number is {num}")

```

# Python compound interest

```
principle = 0
rate = 0
time = 0

while True :
    principle = float(input("Enter the principle amount:"))
    if principle < 0:
        print("Principle can't be less than zero")
    else :
        break
while True :
    rate = float(input("Enter the interest rate:"))
    if rate < 0:
        print("Interest can't be less than zero")
    else:
        break

while True :
    time = float(input("Enter the time in years:"))
    if time < 0:
        print("Time can't be less than zero")
    else :
        break

total = principle * pow((1 + rate / 100), time)
print(f"Balance after {time} year/s: ${total}:.2f")

```

# for loops
```
# for loops = execute a block of code a fixed number of times
# You can iterate over, string over a range, string, sequence, etc


for x in range(1, 21) :
    if x == 13:
        break
else:
    print(x)

```

# Countdown timer 
```

import time
my_time = int(input("Enter the time in seconds:"))

for x in range(my_time,0 ,-1):
    seconds = x % 60
    minutes = int(x / 60) % 60
    hours =int (x / 3600)
    print(f"{hours:02}:{minutes:02}:{seconds:02}")
    time.sleep(1)
print("Time's up")

```

# Nested loop

```

# Nested loop = A loop within another loop ( outer, inner)
#outer loop :
# inner loop :

rows = int(input("Enter the number # of rows:"))
columns = int(input("Enter the number # of columns:"))
symbol = input(" Enter to symbol to use :")

for x in range (rows) :
    for y in range(columns):
        print(symbol, end="")
    print()

```


# List, Set, Tuple

```

# collection = single "variable" used to store multiple values
# list =[] ordered and changeable, Duplicates OK
# Set = {} unordered and immutable, but Add/Remove Ok,. No duplicate
# Tuple () ordered and unchangeable. Dublicates OK. Faster
# fruits = ["apple", "orange", "banana", "coconut"]
# List

print(fruits[::-1])
    for x in fruits :
     print(x)
print(len(fruits))
print(dir(fruits))

print("Mango" in fruits)
fruits.append("pineapple")
fruits.remove("apple")
fruits.insert(0, "pineapple")
fruits.sort()
fruits.reverse()
fruits.clear()
print(fruits.index("apple"))
print(fruits.count("apple"))
print(fruits)

# Set
fruits = {"apple", "orange", "banana", "coconut"}
print(dir(fruits))
print(len(fruits))
print("Guava" in fruits)
print(fruits[0])
fruits.add("Mango")
fruits.remove("apple")
fruits.pop()
fruits.clear()

print(fruits)

# Tuple
fruits = ("apple", "orange", "banana", "coconut")


print(dir(fruits))
print(len(fruits))
print("Guava" in fruits)
print(fruits.index("apple"))
print(fruits.count("apple"))

for fruit in fruits:
    print(fruit)
```
# Shopping cart program

```

foods = []
prices = []
total = 0

while True:
    food = input("enter a food to buy (q to quit):")
    if food.lower() == "q":
        break
    else:
        price = float(input(f"Enter the price of a {food}: $"))
        foods.append(food)
        prices.append(price)

print("-----Your Cart----- ")

for food in foods :
    print(food, end=" ")

    for price in prices:
        total += price

print()
print(f"Your total is : ${total}")


```


# Python quiz game

```
questions = (("How many elements are in the perodic table?"),
           "Which animal lays the largest egg?",
           "What is the most abundant gas in Earth's atmosphere?",
             "How many bones are in the human body",
           "Which planet in the solar system is the hottest?")

options = (("A. 116", "B. 117", "C. 118", "D.119"),
          ("A. Whale", "B. Crocodile", "C. Elephant", "D. Ostrich"),
          ("A. Nitrogen", "B. Oxygen", "C. Carbon-Dioxide", "D. Hydrogen"),
          ("A. 206", "B. 207", "C. 208", "D.209"),
          ("A. Mercury", "B.Venus", "C. Earth", "D.Mars"))

answers = ("C", "D", "A", "A", "B")
guesses =[]
score = 0
question_no = 0

for question in questions:
    print("------------")
    print(question)
    for option in options[question_no]:
        print(option)

    guess = input("Enter (A,B,C,D:").upper()
    guesses.append(guess)
    if guess == answers[question_no]:
        score+=1
        print("Correct!")
    else:
        print("INCORRECT!")
        print(f"{answers[question_no]} is the correct answer")
    question_no+=1
    print("----------------")
    print("    RESULTS     ")
    print("----------------")

print("answers: ",end="")
for answer in answers:
    print(answer,end=" ")
    print()

print("guesses: ",end="")
for guess in guesses:
    print(guess,end=" ")
    print()

score = (score / len(questions) * 100)
print(f"Your score is :{score}%")

``` 

# Dictionaries

```

# dictionary = a collection of {keu:} value pairs ordered and changeable. No dublicates

capitals = {"USA": "Washington D.C",
            "India": "New Delhi",
            "China": "Beijing",
            "Rusia": "Moscow"}

# print(dir(capitals))
# print(help(capitals))
# print(capitals.get("India"))

# if capitals.get("Rusia"):
#     print("the captial does exists")
# else:
#     print("The capital doesn't exist")
# capitals.update({"Germany": "Berlin"})
# capitals.pop("China")
# capitals.popitem()
# capitals.clear()
# keys = capitals.keys()

# for key in capitals.keys():
#     print(key)

# values = capitals.values()
# for value in capitals.values():
#     print(value)

items = capitals.items()
for key, value  in capitals.items():
    print(f"{key}: {value}")

```
# Concession stand program

```


menu = {"pizza": 3.00,
        "nachos": 4.50,
        "popcorn": 6.00,
        "fires": 2.50,
        "chips": 1.00,
        "burger": 3.50,
        "soda": 3.00,
        "lemonade": 4.25}
cart =[]
total = 0

print("---------MENU---------")
for key, value in menu.items():
    print(f"{key}: ${value:.2f}")
print("---------------------")

while True :
    food = input("Select an item (q to quit):").lower()
    if food == "q":
        break
    elif menu.get(food) is not None:
        cart.append(food)

print("----- Your Order -----")

for food in cart:
    total += menu.get(food)
    print(food, end=" ")

print()
print(f"Total is: {total:.2f}")

```

# Random number 

```
import random

low = 1
high = 100
options = ("rock", "paper", "scissors")
cards = ["2", "3", "4", "5", "6", "7", "8", "9", "10", "j", "Q", "K", "A"]

# number =random.randint(low, high)
# number = random.random()
# options = random.choice(options)
random.shuffle(cards)

print(cards)


```

# Python number guessing game 

```

import random

lowest_num = 1
highest_num = 100
answer = random.randint(lowest_num, highest_num)
guesses = 0
is_running = True

print("Python Number Guessing Game")
print(f"Select a number between {lowest_num} and {highest_num}")

while is_running:
    guess = input("Enter your guess: ")
    if guess.isdigit():
        guess = int(guess)
        guesses += 1

        if guess < lowest_num or guess > highest_num:
            print("That number is out of range")
            print(f"Please select a number between {lowest_num} and {highest_num}")
        elif guess < answer:
            print("Too low! Try again!")
        elif guess > answer:
            print("Too high! Try again!")
        else:
            print(f"CORRECT! The answer was {answer}")
            print(f"Number of guesses: {guesses}")
            is_running = False
    else:
        print("Invalid guess")
        print(f"Please select a number between {lowest_num} and {highest_num}")

```

# Python Rock, Paper, Scissors

```

import random

options = ("rock", "paper", "scissors")

playing = True

while playing:

    player = None
    computer = random.choice(options)

    while player not in options:
        player = input("Enter a choice (rock, paper, scissors): ")

    print(f"Player: {player}")
    print(f"Computer: {computer}")

    if player == computer:
        print("It's a tie!")
    elif player == "rock" and computer == "scissors":
        print("You win!")
    elif player == "paper" and computer == "rock":
        print("You win!")
    elif player == "scissors" and computer =="paper":
        print("You win")
    else:
        print("You lose!")
    if not input("Play again? (y/n): ").lower() == "y":
        playing = False

print("Thanks for playing")

```
# Dice roller program
```
import random
# print("\u25CF \u250C \u2500 \u2510 \u2502 \u2514 \u2518 ")
# ● ┌ ─ ┐ │ └ ┘

# "┌─────────┐"
# "│         │"
# "│         │"
# "│         │"
# "└─────────┘"

dice_art = {
    1: ("┌─────────┐",
        "│         │",
        "│    ●    │",
        "│         │",
        "└─────────┘"),
    2: ("┌─────────┐",
        "│  ●      │",
        "│         │",
        "│      ●  │",
        "└─────────┘"),
    3: ("┌─────────┐",
        "│ ●       │",
        "│    ●    │",
        "│       ● │",
        "└─────────┘"),
    4: ("┌─────────┐",
        "│ ●     ● │",
        "│         │",
        "│ ●     ● │",
        "└─────────┘"),
    5: ("┌─────────┐",
        "│ ●     ● │",
        "│    ●    │",
        "│ ●     ● │",
        "└─────────┘"),
    6:(" ┌─────────┐",
        "│ ●     ● │",
        "│ ●     ● │",
        "│ ●     ● │",
        "└─────────┘"),
}
dice =[]
total = 0
num_of_dice = int(input("How many dice?: "))

for die in range(num_of_dice):
    dice.append(random.randint(1,6))


for line in range(5):
    for die in dice:
        print(dice_art.get(die)[line], end="")
    print()


for die in dice:
    total += die
print(f"total:{total}")

```

# Function

```

# function = A block of resuable code place() after the function name to invoke it


# Example 1
def happy_birthday(name, age):
    print(f"Happy birthday to {name}")
    print(f"You are {age} years old")
    print("Happy birthday to you")
    print()

happy_birthday("bro", 20)
happy_birthday("Steve", 30)
happy_birthday("Buffon", 60)


# Example 2
def display_invoice(username, amount, due_date):
    print(f"Hello{username}")
    print(f"You bill of {amount:.2f} is due on {due_date}")

display_invoice("BroCode", 42.50, "01/12")

return = statement used to end a function and send a result back to the caller


def add(x, y):
    z = x + y
    return z

def subtract(x, y):
    z = x - y
    return z

def multiply(x, y):
    z = x * y
    return z

def divide(x, y):
    z = x / y
    return z

print(add(1,2))
print(subtract(1,2))
print(multiply(1,2))
print(divide(1,2))


def create_name(first, last):
    first = first.capitalize()
    last = last.capitalize()
    return first +" " + last

full_name = create_name("pratyush", "maharjan")

print(full_name)

```