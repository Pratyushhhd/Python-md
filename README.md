# Python-md

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


# Default arguments
```

from dis import disco


# def net_price(list_price, discount=0, tax = 0.05):
#     return list_price * (1 - discount) * (1 + tax)

# print(net_price(500))
# print(net_price(500, 0.1))
# print(net_price(500, 0.1, 0))

import time
def count(end, start=0):
    for x in range(start, end+1):
        print(x)
        time.sleep(1)
    print("DONE!")
count(30, 15)

```

# Keyword argument
```

# def hello(greeting, title, first, last):
#     print(f"{greeting} {title} {first}, {last}")
#
# hello("Hello", title = "Mr", first = "Pratyush", last= "Maharjan")

# for x in range(1, 11):
    # print(x, end=" ")

def get_phone(country, area, first, last):
    return f"{country}-{area}-{first}-{last}"

phone_num = get_phone(country=1, area=123, first=456, last=7890)
print(phone_num)
```
# args and kwargs
```

# Args
def add(*args):
    total = 0
    for arg in args :
        total += arg
    return total
print(add(1, 2, 3))

def display_name(*args):
    for arg in args:
        print(arg, end=" ")

display_name("Dr", "Pratyush", "Maharjan")

# kwargs
def print_address(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_address(street = "123 fake street",
              city ="Detroit",
              state ="MI")


def shipping_label(*args, **kwargs):
    for arg in args:
        print(arg, end=" ")
    print()

    if "apt" in kwargs:
        print(f"{kwargs.get('apt')}")
    elif "pobox" in kwargs:
        print(f"{kwargs.get('street')}")
        print(f"{kwargs.get('pobox')}")

    else:
        print(f"{kwargs.get('street')}")

    print(f"{kwargs.get('city')}")
    print(f"{kwargs.get('state')}")



shipping_label("Dr", "Spongebob", "Squarepants", "III",
               street = "123 fake street",
               pobox = "787",
               city="Detroit",
               state ="MI")

```

# iterable
```

# iterables = An object/collection that can return its elements one at a time, allowing it  to be iterated over in a loop

numbers =(1, 2, 3, 4, 5)

for number in reversed(numbers):
    print(number, end=" - ")

name ="Pratyush Maharjan"

for character in name:
        print(character, end=" ")

my_dictionary = {"A": 1, "B": 2, "C": 3 }

for key ,value in my_dictionary.items():
    print(f"{key} = {value}" )

```


# Membership operator
```
 word = "APPLE"
 letter = input("Guess a letter in the secret word: ")

 if letter not in word:
     print(f"{letter} was not found")
 else :
     print(f"There is a {letter}")

 students = {"Spongerbob","Patrick", "Sandy"}

 student = input("Enter the name of a student: ")

 if student not in students:
    print(f"{student} was not found")
 else:
     print(f"{student} is a student")


 grades = {"Sandy": "A", "Patrick": "B", "Spongebob": "C", "Squidward": "D"}

 student = input("Enter the name of a student:")

 if student in grades:
     print(f"{student}'s grade is {grades[student]}")
 else:
     print(f"{student} was not found")


email ="pratyushmaharjan90@gmail.com"

if  "@" in email and "." in email:
    print("Valid email")
else:
    print("Invalid email")

```

# List comprehension 
```

# list comprehension = A concise way to create list in Python
#                   Compact and easier to read than traditional loops
#                       [expression for value in iterable if condition ]

doubles = [x * 2 for x in range (1,11)]
triples = [y * 3 for y in range (1, 11)]
squares = [z * z for z in range (1, 11)]

print(squares)

fruits = ["apple", "orange", "banana", "coconut"]
fruits_char = [fruit[0] for fruit in fruits]

print(fruits_char)


numbers = [1, -2, 3, -4, 5, -6, -7, 8]
positive_num = [num for num in numbers if num >= 0]
negative_num = [num for num in numbers if num < 0]
even_num = [num for num in numbers if num % 2 == 0]
odd_num = [num for num in numbers if num % 2 == 1]


print(odd_num)


grades = [85, 42, 79, 90, 56, 61, 30]
passing_grades = [grade for grade in grades if grade >= 60]

print(passing_grades)

```

# Match-case statemnent

```
def is_weekend(day):
    match day:
        case "Saturday" |"Sunday":
            return True
        case "Monday" | "Tuesday" | "Wednesday" | "Thrusday" | "Friday":
            return False
        case _:
            return False

print(is_weekend("Monday"))

```

# Module

```
# import math
# # import math as m
# # from math import e
# a, b, c, d, e = 1, 2, 3, 4, 5
#
# print(math.e ** a)
# print(math.e ** b)
# print(math.e ** c)
# print(math.e ** d)
# print(math.e ** e)

import Example

result = Example.pi
result = Example.square(3)
result = Example.circumference(3)
result = Example.area(3)


print(result)

--------------------

pi = 3.14159

def square(x):
    return x ** 2
def cube(x):
    return x ** 3
def circumference(radius):
    return 2 * pi * radius
def area (radius):
    return pi * radius ** 2


```

# Scope resolution

```
# variable scope = where a variable is visible and accessible
# scope resolution = (LEGB) Local -> Enclosed -> Global -> Built-in

def func1():
    x = 1
    def func2():
        print(x)

    func2()


func1()


def func1():
    print(x)
def func2():
    print(x)

x = 3

func1()
func2()


from math import e
def func1():
    print(e)

e = 3

func1()
```

# if name ==' main '
## Script 1
```
# if_name ==_ main__: (this secret can be impoerted OR run standlone Functions and classes in this module can be reused without the main block of code executing)


def favorite_food(food):
    print(f"Your favorite food is {food}")

def main():
    print("This is script 1")
    favorite_food("Pizza")
    print("Goodbye")


if __name__ == '__main__':
    main()
```
## Script 2
```

from script1 import *

def favorite_drink(drink):
    print(f"Your favorite drink is {drink}")

print("This is script2")
favorite_food("Sushi")
favorite_drink("Coffee")
print("Goodbye!")

```

# Banking Program

```
def show_balance(balance):
    print("***********************")
    print(f"Your Balance is ${balance:.2f}")
    print("***********************")

def deposit():
    print("***********************")
    amount = float(input("Enter the amount to be deposited: "))
    print("***********************")

    if amount < 0 :
        print("***********************")
        print("That's not a valid amount")
        print("***********************")
        return 0
    else:
        return amount
def withdraw(balance):
    print("***********************")
    amount = float(input("Enter amount to be withdrawn: "))
    print("***********************")

    if amount > balance:
        print("***********************")
        print("Insufficient funds")
        print("***********************")

    elif amount < 0:
        print("***********************")
        print("Amount must be greater than 0")
        print("***********************")
        return 0
    else:
        return amount

def main():
    balance = 0
    is_running = True

    while is_running:
        print("***********************")
        print("    Banking Program    ")
        print("***********************")
        print("1. Show Balance")
        print("2. Deposit!")
        print("3. Withdraw")
        print("4. Exit")
        print("***********************")

        choice = input("Enter your choice (1-4): ")

        if choice == '1':
            show_balance(balance)
        elif choice =='2':
            balance += deposit()
        elif choice =='3':
            balance -= withdraw(balance)
        elif choice =='4':
            is_running =False
        else:
            print("***********************")
            print("That is not a valid choice")
            print("***********************")

    print("***********************")
    print("Thank you! Have a nice day")
    print("***********************")


if __name__ == '__main__':
    main()

```

# Slot Game

```
import random

def spin_row():
    symbols = ['🍒', '🍉', '🍋', '🔔', '⭐']
    return [random.choice(symbols) for _ in range(3)]

def print_row(row):
    print("***********************")
    print(" | ".join(row))
    print("***********************")

def get_payout(row, bet):
    if row[0] == row[1] == row[2]:
        if row[0] == '🍒':
            return bet * 3
        elif row[0] == '🍉':
            return bet * 4
        elif row[0] == '🍋':
            return bet * 5
        elif row[0] == '🔔':
            return bet * 10
        elif row[0] == '⭐':
            return bet * 20
    return 0

def main():
    balance = 100

    print("***********************")
    print("Welcome to Python Slots")
    print("Symbols: 🍒 🍉 🍋 🔔 ⭐")
    print("***********************")

    while balance > 0:
        print(f"Current balance: ${balance}")

        bet = input("Place your bet amount: ")

        if not bet.isdigit():
            print("Please enter a valid number.")
            continue

        bet = int(bet)
        if bet > balance:
            print("Insufficient funds.")
            continue
        if bet <= 0:
            print("Bet must be greater than 0.")
            continue

        balance -= bet

        row = spin_row()
        print("Spinning...\n")
        print_row(row)

        payout = get_payout(row, bet)
        if payout > 0:
            print(f"You won ${payout}!")
        else:
            print("Sorry, you lost this round.")

        balance += payout

        if balance <= 0:
            break

        play_again = input("Do you want to spin again? (Y/N): ").strip().upper()
        if play_again != 'Y':
            break

    print("******************************************")
    print(f"Game over! Your final balance is ${balance}")
    print("******************************************")

if __name__ == '__main__':
    main()

```

# Encryption program
```
import random
import string
from operator import index

chars = " " + string.punctuation + string.digits + string.ascii_letters
chars = list(chars)
key = chars.copy()

random.shuffle(key)
# print(f"chars: {chars}")
# print(f"key: {key}")


#Encrypt

plain_text = input("Enter a message to encrypt: ")
cipher_text = " "

for letter in plain_text:
    index = chars.index(letter)
    cipher_text += key[index]

print(f"orignal message: {plain_text}")
print(f"encrypted message: {cipher_text}")

#Decrypt

cipher_text = input("Enter a message to encrypt: ")
plain_text = " "

for letter in cipher_text:
    index = key.index(letter)
    plain_text += chars[index]

print(f"encrypted message: {cipher_text}")
print(f"orignal message: {plain_text}")

```

# Hangman game in Python

```
from words_list import words
import random

#dictionary of key:()
hangman_art = {0: ("   ",
                   "   ",
                   "   "),
               1: (" o ",
                   "   ",
                   "   "),
               2: (" o ",
                   " | ",
                   "   "),
               3: (" o ",
                   "/| ",
                   "   "),
               4: (" o ",
                   "/|\\",
                   "   "),
               5: (" o ",
                   "/|\\",
                   "/  "),
               6: (" o ",
                   "/|\\",
                   "/ \\")}

def display_man(wrong_guesses):
    print("**********")
    for line in hangman_art[wrong_guesses]:
        print(line)
    print("**********")


def display_hint(hint):
    print(" ".join(hint))

def dsiplay_answer(answer):
    print(" ".join(answer))

def main():
    answer = random.choice(words)
    hint = ["_"] * len(answer)
    wrong_guesses = 0
    guessed_letters = set()
    is_running = True

    while is_running :
        display_man(wrong_guesses)
        display_hint(hint)
        guess = input("Enter a letter: ").lower()

        if len(guess) != 1 or not guess.isalpha():
            print("Invalid input")
            continue
        if guess in guessed_letters:
            print(f"{guess} is already guessed")
            continue

        guessed_letters.add(guess)

        if guess in answer:
            for i in range(len(answer)):
                if answer[i] == guess:
                    hint[i] = guess

        else:
            wrong_guesses += 1
        if "_" not in hint:
            display_man(wrong_guesses)
            dsiplay_answer(answer)
            print("YOU WIN !")
            is_running = False
        elif wrong_guesses >= len(hangman_art) - 1 :
            display_man(wrong_guesses)
            dsiplay_answer(answer)
            print("YOU LOSE!")
            is_running = False

if __name__ == '__main__':
    main()


```
## Word_list
```
# word for hangman game

words = ("aardvark", "alligator", "alpaca", "ant", "anteater", "antelope", "ape", "armadillo", "baboon", "badger", "bat", "bear", "beaver", "bee", "bison", "boar", "buffalo", "butterfly", "camel", "capybara", "caribou", "cat", "caterpillar", "cattle", "chamois", "cheetah", "chicken", "chimpanzee", "chinchilla", "chough", "clam", "cobra", "cockroach", "cod", "coyote", "crab", "crane", "crocodile", "crow", "curlew", "deer", "dinosaur", "dog", "dogfish", "dolphin", "donkey", "dormouse", "dotterel", "dove", "dragonfly", "duck", "dugong", "dunlin", "eagle", "echidna", "eel", "elephant", "elephant-seal", "elk", "emu", "falcon", "ferret", "finch", "fish", "flamingo", "fly", "fox", "frog", "gaul", "gazelle", "gerbil", "giant-panda", "giraffe", "gnat", "gnu", "goat", "goldfinch", "goldfish", "goose", "gorilla", "goshawk", "grasshopper", "grouse", "guanaco", "gull", "hamster", "hare", "hawk", "hedgehog", "heron", "herring", "hippopotamus", "hornet", "horse", "human", "hummingbird", "hyena", "ibex", "ibis", "jackal", "jaguar", "jay", "jellyfish", "kangaroo", "kingfisher", "koala", "komodo-dragon", "kookaburra", "kouprey", "kudu", "lapwing", "lark", "lemur", "leopard")

```

# Python Oop

```
from car import Car

car1 = Car("Mustang", 2024, "black", False)
car2 = Car("Corvette", 2025, "blue",True)
car3 = Car("Tesla", 2025, "grey",True)


# print(car2.model)
# print(car2.year)
# print(car2.color)
# print(car2.for_sale)

car1.describe()
```
## car 

```
class Car:
    def __init__(self, model, year, color, for_sale):
        self.model = model
        self.year = year
        self.color = color
        self.for_sale = for_sale
    def drive(self):
        print(f"You drive the {self.color}{self.model}")

    def stop(self):
        print(f"You stop the {self.color} {self.model}")

    def describe(self):
        print(f"{self.year} {self.color} {self.model}")

```

# Class Variables

```

class Student:

    class_year = 2028
    num_student = 0

    def __init__(self, name, age):
        self.name = name
        self.age = age
        Student.num_student += 1

student1 = Student("Spongebob", 30)
student2 = Student("Patrick", 35)
student3 = Student("Squidward",55)
student4 = Student("Sandy",27)

# print(student2.name)
# print(student2.age)
# print(Student.class_year)
print(f"My graduating class of {Student.class_year} has { Student.num_student} students.")
print(student1.name)
print(student2.name)
print(student3.name)
print(student4.name)

```

# Inheritance

```

class Animal:
    def __init__(self, name):
        self.name = name
        self.is_alive = True

    def eat(self):
            print(f"{self.name} is eating")

    def sleep(self):
            print(f"{self.name} is sleeping")

class Dog(Animal):
    def speak(self):
        print("WOOF")
class Cat(Animal):
    def speak(self):
        print("MEOW")
class Mouse(Animal):
    def speak(self):
        print("SQUEEK")
dog = Dog("Scooby")
cat =Cat("Garfield")
mouse = Mouse("Mickey")

print(dog.name)
print(dog.is_alive)
dog.eat()
dog.sleep()
dog.speak()

```
# Multiple inheritance

```
class Animal :

    def __init__(self, name):
        self.name = name


    def eat(self):
        print(f"{self.name} is eating")
    def sleep(self):
        print(f"{self.name} is sleeping")
class Prey(Animal):
    def flee(self):
        print(f"{self.name} is fleeing")
class Predator(Animal):
    def hunt(self):
        print(f"{self.name} is hunting")


class Rabbit(Prey):
    pass

class Hawk(Predator):
    pass

class Fish(Prey, Predator):
    pass

rabbit = Rabbit("Bugs")
hawk = Hawk("Tony")
fish = Fish("Nemo")


fish.sleep()

```
# Super ( )

```
from random import triangular


class Shape:
    def __init__(self,color, is_filled):
        self.color = color
        self.is_filled = is_filled
    def describe(self):
        print(f"It is {self.color} and {'filled' if self.is_filled else 'not filled'}")

class Circle(Shape):
    def __init__(self, color, is_filled, radius):
        super().__init__(color, is_filled)
        self.radius =radius

    def describe(self):
        super().describe()
        print(f"It is a circle with an area of {3.14 * self.radius * self.radius} cm^2")


class Square(Shape):
    def __init__(self, color, is_filled, width):
        super().__init__(color, is_filled)
        self.width = width

    def describe(self):
        super().describe()
        print(f"It is a square with an area of {self.width * self.width} cm^2")

class Triangle(Shape):
    def __init__(self, color, is_filled, width, height):
        super().__init__(color, is_filled)
        self.width = width
        self.height = height

    def describe(self):
        super().describe()
        print(f"It is a triangle with an area of {self.width * self.height / 2} cm^2")

circle = Circle("blue", True, 5)
square = Square("red", True, 6)
triangle = Triangle("green", True, 5, 8)

# print(triangle.color)
# print(triangle.is_filled)
# print(f"{triangle.width}cm")
# print(f"{triangle.height}cm")

triangle.describe()

```

# Polymorphism

```
from abc import ABC, abstractmethod

class Shape:
    @abstractmethod
    def area(self):
        pass



class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    def area(self):
        return 3.14 * self.radius


class Square(Shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        return  self.side ** 2


class Triangle(Shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height

    def area(self):
        return self.base * self.height * 0.5

class Pizza(Circle):
    def __init__(self, topping, radius):
        super().__init__(radius)
        self.topping = topping

shapes = [Circle(4), Square(5), Triangle(6,7), Pizza("pepperoni", 25)]


for shape in shapes:
    print(f"{shape.area()}cm²")

```

# Duck typing 
```

class Animal:
    alive = True

class Dog(Animal):
    def speak(self):
        print("WOOF!")

class Cat(Animal):
    def speak(self):
        print("MEOW!")
class Car:
    alive = False
    def speak(self):
        print("HONK!")


animals = [Dog(), Cat(), Car()]

for animal  in animals:
    animal.speak()iiii
    print(animal.alive)

```
# Static Method

```
class Employee:

    def __init__(self, name, position):
        self.name = name
        self.position = position

    def get_info(self):
        return f"{self.name} = {self.position}"
    @staticmethod
    def is_valid_position(position):
        valid_positions = ["Manager", "Cashier", "Cook", "Janitor"]
        return position in valid_positions

employee1 = Employee("Eugune", "Manager")
employee2 = Employee("Squidward", "Cashier")
employee3 = Employee("Spongebob", "Cook")

print(Employee.is_valid_position("manager"))
print(employee1.get_info())
print(employee2.get_info())
print(employee3.get_info())


```



# Class Method

```



class Student:

    count = 0
    total_gpa = 0

    def __init__(self, name, gpa):
        self.name = name
        self.gpa = gpa
        Student.count += 1
        Student.total_gpa += gpa

    def get_info(self):
        return f"{self.name} {self.gpa}"

    @classmethod
    def get_count(cls):
        return f"Total # of student: {cls.count}"

    @classmethod
    def get_average_gpa(cls):
        if cls.count == 0:
            return 0
        else:
            return f"average gpa:{cls.total_gpa / cls.count:.2f}"
student1 = Student("Spongebob", 3.2)
student2 = Student("Patrick", 2.0)
student3 = Student("Sandy", 4)

print(Student.get_count())
print(Student.get_average_gpa())


```

# Magic Method

```

class Book:
    def __init__(self, title, author, num_pages):
        self.title = title
        self.author = author
        self.num_pages = num_pages

    def __str__(self):
        return f"{self.title} by {self.author}"

    def __eq__(self, other):
        return self.title == other.title and  self.author == other.title

    def __lt__(self, other):
        return self.num_pages < other.num_pages

    def __gt__(self, other):
        return self.num_pages > other.num_pages

    def __add__(self, other):
        return f"{self.num_pages + other.num_pages} pages"

    def __contains__(self, keyword):
        return keyword in self.title or keyword in self.author

    def __getitem__(self, key):
        if key == "title":
            return self.title
        elif  key == "author":
            return self.author
        elif key == "num_pages":
            return self.num_pages
        else:
            return f"Key {key} was not found"
book1 = Book ("The Hobbit", "J.R.R Tolkien", 310)
book2 = Book ("Harry Potter and The Philosopher", "J.K Rowling", 223)
book3 = Book ("Then Lion and the Wardrobe", "C.S. Lewis", 117)

print(book3)
print(book1 == book2)
print(book2 < book3)
print(book2 > book3)
print(book2 + book3)
print("Lion" in book3)
print(book1 ['title'])
print(book3['audio'])

```

# Property 

```




class Rectangle:
    def __init__(self, width, height):
        self._width = width
        self._height = height

    @property
    def width(self):
        return f"{self._width:.1f}cm"

    @property
    def height(self):
        return f"{self._height:.1f}cm"

    @width.setter
    def width(self, new_width):
        if new_width > 0 :
            self._width = new_width
        else:
            print("Width must be greater than zero")

    @height.setter
    def height(self, new_height):
        if new_height > 0:
            self._height = new_height
        else:
            print("Height must be greater than zero")
    @width.deleter
    def width(self):
        del self._width
        print("Width has been deleted")

    @height.deleter
    def height(self):
        del self._height
        print("Height has been deleted")

rectangle = Rectangle(3,4)


rectangle.width = 5
rectangle.height = 6

del rectangle.width
del rectangle.height

```

# Decorator

```


def add_sprinkles(func):
    def wrapper(*args, **kwargs):
        print("* You add sprinkles *")
        func(*args, **kwargs)
    return wrapper

def add_fude(func):
    def wrapper(*args, **kwargs):
        print("* You add fudge *")
        func(*args, **kwargs)
    return wrapper

@add_sprinkles
@add_fude

def get_ice_cream(flavor):
    print(f"Here is your {flavor} icecream")


get_ice_cream("Vanilla")

```
# Exception handlying

```


try:
    number = int(input("Enter a number: "))
    print(1 / number)
except ZeroDivisionError:
    print("You can't divide by zero")

except ValueError:
    print("Enter only numbers please!")

except Exception:
    print("Something went wrong")

finally:
    print("Do some cleanup!")

```

# File detection 

```



import os

file_path = "C:/Users/WELCOME/Desktop/test"

if os.path.exists(file_path):
    print(f"The location '{file_path}' exists")
    if os.path.isfile(file_path):
        print("That is a file")
    elif os.path.isdir(file_path):
        print("That is a directory")

else:
    print("The location doesn't exists")

```

# writing file

## .txt

```
employees = ["Eugene", "Squidward", "Spongebob", "Patrick"]

file_path = "C:/Users/WELCOME/Desktop/output.txt"

try:
    with open(file_path, "a") as file:
        for employee in employees:
            file.write("\n" + employee)
        print(f"txt file '{file_path}' was created")

except FileExistsError:
    print("That file already exists")
```
## json

```
import json
employee = {
    "name": "Spongebob",
    "age" : "30",
    "job" : "cook"
}
file_path = "C:/Users/WELCOME/Desktop/output.json"

try:
    with open(file_path, "w") as file:
        json.dump(employee, file, indent=4)
        print(f"json file '{file_path}' was created")

except FileExistsError:
    print("That file already exists")
```

## csv

```

import csv

employees = [["Name", "Age", "Job"],
            ["Spongebob", 30, "Cook"],
            ["Patrick", 37, "Unemployed"],
            ["Sandy", 27, "Scientist"]]
file_path = "C:/Users/WELCOME/Desktop/output.csv"

try:
    with open(file_path, "w", newline= "") as file:
        writer = csv.writer(file)
        for row in employees:
            writer.writerow(row)
        print(f"csv file '{file_path}' was created")

except FileExistsError:
    print("That file already exists")

```

# reading file

## .txt

```
file_path = "C:/Users/WELCOME/Desktop/input.txt"

try:
    with open(file_path, "r") as file:
        content = file.read()
        print(content)

except FileNotFoundError:
    print("That file was not found")

except PermissionError:
    print("You do not have permission to read that file")
```

## json

```
import json
file_path = "C:/Users/WELCOME/Desktop/output.json"

try:
    with open(file_path, "r") as file:
        content = json.load(file)
        print(content["name"])

except FileNotFoundError:
    print("That file was not found")

except PermissionError:
    print("You do not have permission to read that file")


```

## csv 

```

import csv
file_path = "C:/Users/WELCOME/Desktop/output.csv"

try:
    with open(file_path, "r") as file:
        content = csv.reader(file)
        for line in content:
            print(line)

except FileNotFoundError:
    print("That file was not found")

except PermissionError:
    print("You do not have permission to read that file")

```

# dates and times

```


import datetime

date = datetime.date(2025, 1, 12)
today = datetime.date.today()

time = datetime.time(12, 30, 0)
now = datetime.datetime.now()

now= now.strftime("%H:%M:%S %m-%d-%y")

target_datetime = datetime.datetime(2020, 1, 2, 12, 30, 3)
current_datetime = datetime.datetime.now()

if target_datetime < current_datetime:
    print("Target date has already passed")
else:
    print("Target has NOT passed")

```

# Alarm clock

```

import time
import datetime
import pygame

def set_alarm(alarm_time):
    print(f"Alarm set for {alarm_time}")
    sound_file = "Stuff/MA MARE PANI SWAR  Swapnil Sharma, Rohit Shakya & Gautam Tandukar.mp3"
    is_running = True
    while is_running:
        current_time = datetime.datetime.now().strftime("%H:%M:%S")
        print(current_time)
        if current_time == alarm_time:
            print("WAKE UP!!!")

            pygame.mixer.init()
            pygame.mixer.music.load(sound_file)
            pygame.mixer.music.play()

            while pygame.mixer.music.get_busy():
                time.sleep(1)

            is_running = False

        time.sleep(1)

if __name__ == "__main__":
    alarm_time = input("Enter the alarm time (HH:MM:SS): ")
    set_alarm(alarm_time)
```


# Multithreading

```



import threading
import time

def walk_dog(first):
    time.sleep(8)
    print(f"You finish walking {first}")
def take_out_trash():
    time.sleep(2)
    print("You take out the trash")
def get_mail():
    time.sleep(4)
    print("You get the mail")
chore1 = threading.Thread(target=walk_dog, args=("Scooby",))
chore1.start()

chore2 = threading.Thread(target = take_out_trash)
chore2.start()

chore3 = threading.Thread(target=get_mail)
chore3.start()

chore1.join()
chore2.join()
chore3.join()

print("All chores are complete")


```

# request api
```



import requests

base_url = "https://pokeapi.co/api/v2/"

def get_pokemon_info(name):
    url = f" {base_url}/pokemon/{name}"
    response = requests.get(url)
    print(response)

    if response.status_code == 200:
        pokemon_data =response.json()
        return pokemon_data
    else:
        print(f"Failed to retrieve data {response.status_code}")


pokemon_name = "greninja"

pokemon_info = get_pokemon_info(pokemon_name)

if pokemon_info:
    print(f"Name:{pokemon_info["name"].capitalize()}")
    print(f"Id :{pokemon_info["id"]}")
    print(f"Height: {pokemon_info["height"]}")
    print(f"weight: {pokemon_info["weight"]}")

```

# PyQt5 GUI

```


import sys
from PyQt5.QtWidgets import QApplication, QMainWindow
from PyQt5.QtGui import QIcon


class MainWindow(QMainWindow):
    def __init__(self):
        super().__init__()
        self.setWindowTitle("My first GUI")
        self.setGeometry(300, 100, 500, 500)
        self.setWindowIcon(QIcon("Stuff/WhatsApp Image 2025-08-15 at 3.56.18 PM (1).jpeg"))

def main():
    app = QApplication(sys.argv)
    window = MainWindow()
    window.show()
    sys.exit(app.exec_())

if __name__ == "__main__":
    main()


```
