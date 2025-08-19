# python

# Python 
## variables
## Strings
```
first_name = "Binod"
food = "Pizza"

print(f"Hello {first_name}")
print(f"You like {food}")
```
## Integers
```
age = 20
quantity = 5

print(f"You are {age} years old")
print(f"You are buying {quantity} items.")
```
## Float
```
gpa = 3.2
price = 9.99
distance = 5.5

print(f"Your gpa is {gpa}")
print(f"This item is ${price}")
print(f"You ran {distance} km")
```
## Boolean
```
for_sale = True
if for_sale :
     print("That item is for sale")
else:
     print("That item is NOT available")
```
## type casting
```
name = "Binod"
age = 20
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

## Exercise-3 Madlibs game
```
adjective1 = input("Enter an ajdective (description): ")
noun1 = input("Enter a noun(person, place , thing: "))
adjective2 = input("Enter an ajdective (description): ")
verb1 = input("Enter a verb with 'ing'")
adjective3 = input("Enter an ajdective (description): ")



print(f"Today I went to a {adjective1} zoo.")
print(f"In an exhibit, I saw a {noun1}")
print(f"{noun1} was {adjective2} and {verb1}")
print(f"I was {adjective3}!")
```
## Arithmetic and math
```
x = 3.54
y = 5
z = 8

result = round(x)
result = abs(y)
result = pow(4, 3)
result = max(x, y, z)
result = min(x, y, z)

print(result)
```
## import math
```
x = 9.9

 print(math.pi)
 print(math.e)
 result = math.sqrt(x)
 result = math.ceil(x)
 result = math.floor(x)

 print(result)
```

## exercise-1
```
import math
circumference of circle
radius = float(input('Enter the radius of a circle: '))
circumference = 2 * math.pi * radius

print(f"The circumference is: {round(circumference, 2)}cm")
```
## exercise-2
```
area of circle

radius = float(input('Enter the radius of a circle: '))
area = math.pi * pow(radius, 2)

print(f"the area of a circle is: {round(area, 2)}cm²")

```
## Exerxise-3.
```
a = float(input("Enter side A: "))
b = float(input("Enter side B: "))

c = math.sqrt(pow(a, 2) + pow(b, 2))
print(f"side c = {c}")
```
 ## Exercise-1 Area of rectangle
```
length = float(input("Enter the length: "))
width = float(input("Enter the width: "))
area = length * width

print(f"The area is : {area} cm")
```     

## Exercise-2 Shopping cart program
```
item = input("What item would you like to buy?: ")
price = float(input("What is the price?: "))
quantity = int(input("How many would you like?: "))
total = price * quantity

print(f"YOu have bought {quantity} x {item}/s")
print(f"your total is ${total}")
```


# If statement
```
age = int(input("Enter your age: "))

if age >= 100:
    print("You are too old to sign up")
elif age >= 18:
    print("You are sign up!")
elif age <= 0:
    print("You haven't born yet")
else:
    print("You must be 18+ to sign up")
```
## Python Calculator

```
operator = input("Enter an operator (+ - * /): ")
num1 = float(input("Enter the 1st number: "))
num2 = float(input("Enter the 2nd number: "))

if operator == "+":
    result = num1 + num2
    print(round(result, 3))
elif operator == "-":
    result = num1 - num2
    print(round(result, 3))
elif operator == "*":
    result = num1 * num2
    print(round(result, 3))
elif operator == "/":
    result = num1 / num2
    print(round(result, 3))
else:
    print(f"{operator} is not valid operator")
```    
## python weight converter
```
weight = float(input("Enter your weight: "))
unit = input("Kilograms or pounds? (K or L): ")

if unit == "k":
    weight = weight * 2.205
    unit = "lbs."
    print(f"Your weight is: {round(weight, 1)} {unit}")
elif unit == "l":
    weight = weight / 2.205
    unit = "kgs."
    print(f"Your weight is: {round(weight, 1)} {unit}")
else:
    print(f"{unit} was not valid")
```
# Temperature
```
unit = input("Is this temperature in celsius or fahrenheit (C/F): ")
temp = float(input("Enter the temperature: "))

if unit == "C":
    temp = round((9 * temp) / 5 + 32, 1)
    print(f"The temperature in fahrenheit is: {temp}°F")
elif unit == "F":
    temp = round((temp - 32) * 5 / 9, 1)
    print(f"The temperature in celsius is: {temp}°C")
else:
    print(f"{unit} is an invalid unit of measurement")
```

## Logical operators
```
temp = 28
is_sunny = False

if temp >= 28 and is_sunny:
    print("It is HOT outside")
    print("It is SUNNY")
elif temp <= 0 and is_sunny:
    print("It is COLD outside")
    print("It is SUNNY")
elif 28 > temp > 0 and is_sunny:
    print("It is WARM outside ")
    print("It is SUNNY")
elif temp >= 28 and not is_sunny:
    print("It is HOT outside")
    print("It is CLOUDY")
elif temp <= 0 and not is_sunny:
    print("It is COLD outside ")
    print("It is CLOUDY ")
elif 28 > temp > 0 and not is_sunny:
    print("It is WARM outside")
    print("It is CLOUDY")
```    
## Conditional expression
### A one-line shortcut for the if-else statement 
```
num = 4
a = 6
b = 7
age = 20
temp = 20
user_role = "admin"


 print("positive" if num > 0 else "negative")
 result = "EVEN " if num % 2 == 0 else "ODD"
 max_num = a if a > b  else b
 min_num = a if a < b  else b
 status = "adult" if age >= 20 else "Child"
 weather = "HOT" if temp >= 20 else "COlD"
access_level = "Full Access" if user_role == "admin" else "Limited Access"
print(access_level)
```
## string methods
```
name = input("Enter your full name: ")
phone_number = input("Enter your phone #: ")
result = len(name)
result = name.find("n")
result = name.rfind("i")

name = name.capitalize()
name = name.upper()
name = name.lower()
result = name.isdigit()
result = name.isalnum()
result = phone_number.count("-")
result = phone_number.replace("-", "")
```
```
username = input("Enter your username: ")

if len(username) > 12:
    print("Your username can't be more than 12 character")
elif not username.find(" ") == -1:
    print("Your username can't contain spaces")
elif not username.isalpha():
    print("Your username can't contain numbers")
else:
    print(f"Welcome {username}")
```
# String Indexing 
## Exercise-1
```
credit_number = "1234-5678-9012-3456"
last_digits = credit_number[-4:]
print(f"xxxx-xxxx-xxxx-{last_digits}")
```
## Exercise-2
```
from dis import print_instructions

credit_number = "1234-5678-9012-3456"

credit_number = credit_number[::-1]
print(credit_number )
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

## While loops
Example-1
```


name = input("Enter your name: ")

 while name == "":
     print("You did not enter your name")
     name = input("Enter your name: ")
    print(f"hello {name}")
```

Example-2
```
age = int(input("Enter your age: "))

while age < 0 :
    print("Age can't be negative")
    age = int(input("Enter your age: "))

print(f"You are {age} years old")
```
Example-3
```
food = input("Enter a food you like(q to quit): ")

while not food == "q":
    print(f"you like {food}")
    food = input("Enetr another food you like(q to quit): ")

    print("bye")
```
Example-4
```
num = int(input("Enter a number between 1 - 10: "))

while num < 1 or num > 10:
    print(f"{num} is not valid")
    num = int(input("Enter a number between 1 - 10: "))

    print (f"Your number is {num}")
```
# Python compound interest calculator
```
principle = 0
rate = 0
time = 0

while principle <= 0:
    principle = float(input("Enter the principle amount: "))
    if principle <= 0:
        print("Principle can't be less or equal to zero")

while True:
    rate = float(input("Enter the rate : "))
    if rate < 0:
        print("rate can't be less or equal to zero")
    else:
        break

while time <= 0:
    time = float(input("Enter the time: "))
    if time <= 0:
        print("time can't be less or equal to zero")

total = principle * pow((1 + rate / 100), time)
print(f"Balance after {time} year/s: ${total:.2f}")
``` 

## For loops
```
credit_card = "1234-5678-9012-3456"

for x in credit_card:
    print(x)
```
range and reversed
```
for x in reversed(range(1, 11, 3)):    
    print(x)
```
Continue and break
```
for x in range(1, 21):
    if x == 13:
       continue
    else:
        print(x)
```
```
for x in range(1, 21):
    if x == 13:
        break
    else:
        print(x)
```

## Python Countdown timer program
```
import time

my_time = int(input("Enetr the time in second: "))

for x in range(my_time, 0, -1):
    seconds = x % 60
    minutes = int(x / 60) % 60
    hours = int(x / 3600)
    print(f"00:{minutes:02}:{seconds:02}")
    time.sleep(1)

print("Time up!")
```

## Nested loops = a loop within another loop

```
rows = int(input("Enter the # of rows: "))
columns = int(input("Enter the # of columns: "))
symbol = input("Enter a symbol to use: ")


for x in range(rows):
    for y in range(columns):
        print(symbol, end="")
    print()
```    
## lists, sets, tuple
 lists = [ ] ordered and changeable. Duplicates ok.
```
print(dir(fruits))
print(len(fruits))
print("apple" in fruits)
fruits[1] = "pineapple"
fruits.append("pineapple")
fruits.remove("apple")
fruits.insert(0, "pineapple")
fruits.sort()
fruits.reverse()
fruits.clear()
fruits.index("apple")
fruits.count("banana")


print(fruits)

for fruit in fruits:
    print(fruit)
```
# Sets
sets = { } unordered amd immutable. but Add/remove ok. Faster.
```

fruits = {"apple", "orange", "banana", "coconut"}

print(dir(fruits))
print(len(fruits))
print("apple" in fruits)

fruits.add("pineapple")
fruits.remove("apple")
fruits.pop()
fruits.clear()


print(fruits)

for fruit in fruits:
    print(fruit)
```

# tuples
tuple = ( ) ordered and unchangeable. Duplicates ok , Faster.
```
fruits = ("apple", "orange", "banana", "coconut")

print(dir(fruits))
print(len(fruits))
print("apple" in fruits)

print(fruits.index("apple"))
print(fruits.count("coconut"))

print(fruits)

for fruit in fruits:
    print(fruit)
```    

# Shopping cart program
```
foods = []
prices = []
total = 0

while True:
    food = input("Enter a food to buy (q to quit): ")
    if food.lower() == "q":
        break
    else:
        price = float(input(f"Enter the price of a {food}: $"))
        foods.append(food)
        prices.append(price)
print("----YOUR CART----")

for food in foods:
    print(food, end=" ")

for price in prices:
    total += price

    print()
    print(f"Your total is: ${total}")
```
## 2D collection
```

groceries =  [["apple", "banana", "orange", "coconut"],
              ["carrot", "potatoes", "tomato"],
              ["chicken", "fish", "turkey"]]

for collection in groceries:
    for food in collection:
        print(food, end= " ")
    print()
```

## Num pad
```
num_pad = ((1, 2, 3),
            (4, 5, 6),
            (7, 8, 9),
            ("*", 0, "#"))

for row in num_pad:
    for num in row:
        print(num, end=" ")
    print()
```

# Python quiz game
```

questions = ("How many elements are in the periodic table?: ",
             "Which animal lays the largest eggs?: ",
             "What is the most abundant gas in Earth's atmosphere?: ",
             "How many bones are in human body?: ",
             "Which planet in the solar system is the hottest?: ",)

options = (("A. 116", "B. 117", "C. 118", "D. 119"),
           ("A. Whale", "B. Crocodile", "C. Elephant", "D. ostrich"),
           ("A. Nitrogen", "B. Oxygen", "C. carbon-dioxide", "D. Hydrogen"),
           ("A. 206", "B. 207", "C. 208", "D. 209"),
           ("A. Mercury", "B. Venus", "C. Earth", "D. Mars"))

answers = ("C ", "D ", "A ", "A ", "B ")
guesses = []
score = 0
question_num = 0

for question in questions:
    print("-----------")
    print(question)
    for option in options[question_num]:
        print(option)

    guess = input("Enter (A, B, C, D:) ").upper()
    guesses.append(guess)
    if guess == answers[question_num]:
        score += 1
        print("Correct!")
    else:
        print("INCORRECT!")
        print(f"{answers[question_num]} is correct answer")

    question_num += 1

print("---------------")
print("    RESULTS    ")
print("---------------")

print("answers: ", end="")
for answer in answers:
    print(answer, end="")
print()

print("guesses: ", end="")
for guess in guesses:
    print(guess, end="")
print()

score = int(score / len(questions) * 100)
print(f"Your score is: {score}%")
```

# dictionary = a collection of { key:value} pairs
### ordered and changeable.No duplicates
```

capitals = {"USA": "Washington D.C.",
            "Nepal": "Kathmandu",
            "Russia": "Moscow"
            }

print(dir(capitals))
print(help(capitals))
print(capitals.get("USA"))

if capitals.get("Russia"):
    print("That capital exists")
else:
    print("That capital doesn't exist")

capitals.update({"Germany": "Berlin"})
capitals.pop("Nepal")
capitals.popitem()
capitals.clear()

keys = capitals.keys()

for key in capitals.keys():
    print(key)

values = capitals.values()
for value in capitals.values():
    print(value)

items = capitals.items()


for key, value in capitals.items():
    print(f"{key}: {value}")
```

# concession stand program.
```
menu = {"pizza": 3.00,
        "momo": 2.0,
        "fries": 2.00,
        "chips": 1.00,
        "soda": 1.00}

cart = []
total = 0

print("---------MENU---------")
for key, value in menu.items():
    print(f"{key}: ${value:.2f}")
print("-----------------------")

while True:
    food = input("Select an item(q to quit): ").lower()
    if food == "q":
        break
    elif menu.get(food)is not None:
        cart.append(food)
print("-----YOUR ORDER-----")
for food in cart:
    total += menu.get(food)
    print(food, end=" ")

print()
print(f"Total is: ${total:.2f}")
```
## Random numbers
```
import random

low = 1
high = 100
options = ("rock", "paper", "scissors")
card = ["2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K", "A"]

number = random.randint(low, high)
number = random.random()
option = random.choice(options)

random.shuffle(card)

print(card)
```

# Number guessing game
```
import random

lowest_num = 1
highest_num = 100
answer = random.randint(lowest_num, highest_num)
guesses = 0
is_running = True

print("Python Number Guesing Game")
print(f"Select a number between {lowest_num} and {highest_num}")

while is_running:
    guess = input("Enter your guess: ")
    if guess.isdigit():
        guess = int(guess)
        guesses += 1

        if guess < lowest_num or guess > highest_num:
            print("That number is out of range")
            print(f"Please Select a number between {lowest_num} and {highest_num}")
        elif guess < answer:
            print("Too low! Try again!")
        elif guess > answer:
            print("Too high! Try again!")
        else:
            print(f"CORRECT! the answer was {answer}")
            print(f"Number of guesses: {guesses}")
            is_running = False




    else:
        print("Invalid guess")
        print(f"Please Select a number between {lowest_num} and {highest_num}")
```
## Dice Roller Program
import random
```
 print("\u25CF \u250C \u2500 \u2510 \u2502 \u2514 \u2518")

# ● ┌ ─ ┐ │ └ ┘
```
```
"┌─────────┐"
"│         │"
"│         │"
"│         │"
"└─────────┘"

dice_art = {
    1:("┌─────────┐",
       "│         │",
       "│    ●    │",
       "│         │",
       "└─────────┘" ),
    2: ("┌─────────┐",
        "│ ●       │",
        "│         │",
        "│       ● │",
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
    6: ("┌─────────┐",
        "│ ●     ● │",
        "│ ●     ● │",
        "│ ●     ● │",
        "└─────────┘")
}

dice = []
total = 0
num_of_dice = int(input("How many dice?: "))

for die in range(num_of_dice):
    dice.append(random.randint(1, 6))

# for die in range(num_of_dice):
#     for line in dice_art.get(dice[die]):
#         print(line)

for line in range(5):
    for die in dice:
        print(dice_art.get(die)[line], end="")
    print()

for die in dice:
    total += die
print(f"total: {total}")
```




## function = A block of reusable code
###           place () after the function name to invoke it
```
def happy_birthday(x, y):
    print(f"happy birthday to {x}")
    print(f"you are {y} years old")
    print("happy birthday to you")
    print()

happy_birthday("bro", 10)
happy_birthday("binod", 20)
happy_birthday("bob", 30)
from tkinter.filedialog import dialogstates


def display_invoice(username, amount, due_date):
    print(f"hello {username}")
    print(f"your bill of ${amount:.2f} is due : {due_date}")

display_invoice("Binod Maharjan", 100.01," 01/02/03")

```

```

def add(x, y):
    z = x + y
    return z
print(add(1, 2))

def subtract(x, y):
    z = x - y
    return z
print(subtract(1, 2))

def multiply(x, y):
    z = x * y
    return z
print(multiply(1, 2))

def divide(x, y):
    z = x / y
    return z
print(divide(1, 2))
```


```
def create_name(first, last):
    first = first.capitalize()
    last = last.capitalize()
    return first + " " + last

full_name = create_name("spongebob", "squarepants")

print(full_name)
```

## Default arguments = A default value for certain parameters
- default is used when that argument is omitted
- make your function more flexible, reduce # of arguments
1. positional, 2. Default, 3. keyword, 4. arbitrary

```
def net_price(list_prices, discount=0, tax=0.05):
    return list_prices * (1 - discount) * (1 * tax)

 print(net_price(500))
print(net_price(500, 0.1))
```
## exercise-1 default arguments
```
import time
def count(end, start=0):
    for x in range(start, end+1):
        print(x)
        time.sleep(1)
    print("DONE!")
count(10)
```


## Keyword arguments = an argument preceded by an identifier,helps with readability,order of argument doesn't
```

def hello(greeting, title, first, last):
    print(f"{greeting}{title}{first}{last}")

hello("hello ", title="Mr.",last=" Maharjan", first="Binod"  )
```

### example-1
```
def get_phone(country, area, first, last):
    return f"{country}-{area}-{first}-{last}"

phone_num = get_phone(country=977, area=983, first=456, last=7890)
print(phone_num)
```
### example 2
```
for x in range(1, 11):
    print(x, end=" ")
```

## ARBITRARY

### args = allows you to multiply non-key arguments
```
def add(*args):
    total = 0
    for arg in args:
        total += arg
    return total

print(add(1))
```
```
def display_name(*args):
    for arg in args:
        print(arg, end=" ")

display_name("Mr.", "spongebob", "squarepants")
```

### **kwargs = allows you to pass multiply keyword-arguments
 *unpacking operator
```
def print_address(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_address(street="123 fake st.",
              apt="100",
              city="Deroit",
              state="MI",
              zip="54321")
```
```
def shipping_label(*args, **kwargs):
    for arg in args:
        print(arg, end=" ")
    print()
    if "apt" in kwargs:
        print(f"{kwargs.get('street')} {kwargs.get('apt')}  ")
    elif "pobox" in kwargs:
         print(f"{kwargs.get('street')}")
         print(f"{kwargs.get('pobox')}")
    else:
        print(f"{kwargs.get('street')}")

    print(f"{kwargs.get('city')} {kwargs.get('state')}, {kwargs.get('zip')}")
shipping_label("Dr.", "spongebob", "squarepants", "III",
               street="123 fake st.",
               pobox="PO box #1001",
               city="Deroit",
               state="MI",
               zip="54321")
```

## iterables = An object/collection that can return its elements one at a time, allowing it to be iterables over in loop
```

numbers = [1, 2, 3, 4, 5]

for number in reversed(numbers):
    print(number, end=" - ")
```
```
name = "Binod Maharjan"

for character in name:
    print(character, end=" ")
```
```
my_dictionary = {"A": 1, "B": 2, "C": 3}

for key, value in my_dictionary.items():
    print(f"{key} = {value}")
```

## Membership operators = used to test whether a value or variable is found in a sequence (string, list, set, fictionary)
1. in
2. not in

- string
```
word = "APPLE"

letter = input("Guess the secret word: ")

if letter not in word:
    print(f"{letter} was not found")
else:
    print(f"There is a {letter}")
```
- sets
```
students = {"Ram", "Hari", "Shyam"}

student = input("Enter the name of a student: ")

if student not in students:
    print(f"{student} was not found")
else:
    print(f"{student} is a student")
```
- dictionary
```
grades = {"sandy": "A",
          "Binod": "B",
          "patrick": "C",
          "Spongebob": "D"}

student = input("Enter the name of student: ")

if student in grades:
    print(f"{student}'s grade is {grades[student]}")
else:
    print(f"{student} was mot found")
```
```
email = "Binod123@gmail.com"

if "@" in email and "." in email:
    print("Valid email")
else:
    print("Invalid email")
```
## list comprehension = A concise way to create lists in python
- compact and easier to read than traditional loops
- [expression for value in iterables if condition]
1. Example-1
```
doubles = [x * 2 for x in range(1, 11)]
triples = [y * 3 for y in range(1, 11)]
squares = [z * z for z in range(1, 11)]
print(squares)
```
2. Example-2
```
fruits = ["apple", "orange", "banana", "coconut"]
fruit_char = [fruit[0] for fruit in fruits]
print(fruit_char)
```
3. Example-3
```
numbers = [1, -2, 3, -4, 5, -6, 8, -7]
positive_nums = [num  for num in numbers if num >= 0]
negative_nums = [num  for num in numbers if num < 0]
even_num = [num  for num in numbers if num % 2 == 0]
odd_num = [num  for num in numbers if num % 2 == 1]
print(odd_num)
```
4. Example-4
```
grades = [85, 42, 79, 90, 30, 61]
passing_grades = [garde for garde in grades if garde >= 60]

print(passing_grades)
```

## Module = a file containing code you want to include in your program
- use import to include a module (built-in your own)
- useful to break up a large program reusable separate files

```
module_eg

pi = 3.14159

def square(x):
    return x ** 2
def cube(x):
    return x ** 3

def circumference(radius):
    return 2 * pi * radius

def area(radius):
    return pi * radius ** 2
```
```
import module_eg

result = module_eg.pi
result = result = module_eg.square(3)
result = result = module_eg.cube(3)
result = result = module_eg.circumference(3)
result = result = module_eg.area(3)
print(result)
```

## variable scope = where a variable is visible and accessible
## scope resolution - (LEGB) local -> enclosed -> Built-in

1. Enclosed
```
def func1():
    x = 1

    def func2():
        print(x)
    func2()

func1()
```

2. Global
```
def func1():
    print(x)

def func2():
    print(x)

x = 3

func1()
func2()
```
3. Built-in
```
from math import e

def func1():
    print(e)

e = 3

func1()
```

## if __name__ == '__main__'
- script1
```
def favorite_food(food):
    print(f"Your favorite food is {food}")

def main():
    print("This is script1")
    favorite_food("pizza")
    print("GoodBye!")

if __name__ == '__main__':
    main()
```
- script2
```

from script1 import *

def favorite_drink(drink):
    print(f"Your favorite drink is {drink}")

def main():
    print("This is script2")
    favorite_food("MOMO")
    favorite_drink("coffee")
    print("Goodbye")

if __name__ == '__main__':
    main()

```
##  Python banking program
```
from random import choice
from wsgiref.validate import check_input


def show_balance(balance):
    print("*****************")
    print(f"Your balance is ${balance:.2f}")
    print("*****************")

def deposit():
    amount = float(input("Enter an amount to be deposited: "))

    if amount < 0:
        print("*****************")
        print("That's not a valid amount")
        print("*****************")
        return 0
    else:
        return amount
def withdraw(balance):
    amount = float(input("Enter amount to withdrawn: "))

    if amount > balance:
        print("*****************")
        print("Insufficent funds")
        print("*****************")
        return 0
    elif amount < 0:
        print("*****************")
        print("Amount must be greater than 0")
        print("*****************")
        return 0
    else:
        return amount

def main():

    balance = 0
    is_running = True

    while is_running:
        print("*****************")
        print("Banking program")
        print("*****************")

        print("1. Show Balance")
        print("2. Deposit")
        print("3. Withdraw")
        print("4. Exit")
        print("*****************")

        choice = input("Enter your choice (1-4): ")

        if choice == '1':
            show_balance(balance)
        elif choice == '2':
            balance += deposit()
        elif choice == '3':
            balance -= withdraw(balance)
        elif choice == '4':
            is_running = False
        else:
            print("*****************")
            print("That is not a valid choice")
            print("*****************")
    print("*****************")
    print("Thank you, Have a nice day")
    print("*****************")

if __name__ == '__main__':
    main()
```

## python slot machine
```
import random


def spin_row():
    symbols = ['🍒', '🍉', '🍋', '🔔', '⭐']

    return [random.choice(symbols) for _ in range(3)]

def print_row(row):
    print(" | ".join(row))

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

    print("******************")
    print("Welcome to Python slots")
    print("Symbols: 🍒 🍉 🍋 🔔 ⭐")
    print("*******************")

    while balance > 0:
        print(f"Current balance bet amount: ${balance}")

        bet = input("Place your bet amount: ")

        if not bet.isdigit():
            print("Please enter valid number")
            continue

        bet = int(bet)

        if bet > balance:
            print("Insufficient funds")
            continue

        if bet <= 0:
            print("Bet must be greater than 0")
            continue

        balance -= bet

        row = spin_row()
        print("Spinning...\n")
        print_row(row)

        payout = get_payout(row, bet)

        if payout > 0:
            print(f"You won ${payout}")
        else:
            print("sorry you lost this round")

        balance += payout

        play_again = input("Do you want to spin again? (Y/N): ").upper()

        if play_again != 'Y':
            break

    print(f"Game Over! Your final balance is ${balance}")

if __name__ == '__main__':
    main()
```
## Encryption program
```

import random
import string

chars = " " + string.punctuation + string.digits + string.ascii_letters
chars = list(chars)
key = chars.copy()

random.shuffle(key)

# print(f"cahrs: {chars}")
# print(f"key  : {key}")

#ENCRYPT
plain_text = input("Enter a message to encrypt: ")
cipher_text = ""

for letter in plain_text:
    index = chars.index(letter)
    cipher_text += key[index]

print(f"original mssage: {plain_text}")
print(f"encrypted mssage: {cipher_text}")

#DECRYPT
cipher_text = input("Enter a message to encrypt: ")
plain_text = ""

for letter in cipher_text:
    index = key.index(letter)
    plain_text += chars[index]

print(f"encrypted mssage: {cipher_text}")
print(f"original mssage: {plain_text}")

```

# Hangman program in python

```
# from  wordslist import words/
import random

 words = ("apple", "orange", "banana", "coconut", "pineapple")

# dictionary of key: ()
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
    print("********")
    for line in hangman_art[wrong_guesses]:
        print(line)
    print("********")
def display_hint(hint):
    print(" ".join(hint))

def dispaly_answer(answer):
    print(" ".join(answer))

def main():
    answer = random.choice(words)
    hint = ["_"] * len(answer)
    wrong_guesses = 0
    guessed_letters = set()
    is_running = True

    while is_running:
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
            dispaly_answer(answer)
            print("YOU WIN!!!")
            is_running = False
        elif wrong_guesses >= len(hangman_art) - 1:
            display_man(wrong_guesses)
            dispaly_answer(answer)
            print("YOU LOSE!!!")
            is_running = False


if __name__ == '__main__':
    main()

```
## object = A "bundle" of related attributes (variables ) and methods (function)
- Ex. phone, cup, book
- You need a "class" to create many objects
- class = (blueprint) used to design the structure and layout of an object

```
class car:
    def __init__(self, model, year, color, for_sale):
        self.model = model
        self.year = year
        self.color = color
        self.for_sale = for_sale

    def drive(self):
        print(f"You drive the {self.color} {self.model}")

    def stop(self):
        print(f"you stop the {self.color} {self.model}")

    def describe(self):
        print(f"{self.year} {self.color} {self.model}")
```
```

from Car import car

car1 = car("mustang", 2024, "red", False)
car2 = car("corvette", 2025, "blue", True)
car3 = car("BMW", 2023, "black", False)

# print(car2.model)
# print(car2.year)
# print(car2.color)
# print(car2.for_sale)

# car2.drive()
# car2.stop()

car3.describe()
```

# Class variables = Shared among all instances of a class
- Defined outside the constructor
- Allow you to share among all objects created from that class
```
class Student:

    class_year = 2024
    num_students = 0

    def __init__(self, name, age):
        self.name = name
        self.age = age
        Student.num_students += 1

student1 = Student("spongebob" ,30)
student2 = Student("patrick", 35)
student3 = Student("sandy", 29)
student4 = Student("squidward", 33)



# print(student2.name)
# print(student2.age)
# print(Student.class_year)

print(f"My graduating class of {Student.class_year} has {Student.num_students} students")
print(student1.name)
print(student2.name)
print(student3.name)
print(student4.name)
```

## Inheritance = Allows a class inherit attributes and method from another class
- helps with code reusability and extensibility
- class Child(parent)
```
class animal:
    def __init__(self, name):
        self.name = name
        self.is_alive = True

    def eat(self):
        print(f"{self.name} is eating")

    def sleep(self):
        print(f"{self.name} is sleeping")

class Dog(animal):
    def speak(self):
        print("WOOF")
class Cat(animal):
    def speak(self):
        print("MEOW")
class Mouse(animal):
    def speak(self):
        print("SQUEEK")

dog = Dog("Scooby")
cat = Cat("Tom")
mouse = Mouse("Jerry")

print(dog.name)
print(dog.is_alive)
dog.eat()
dog.sleep()
dog.speak()
```

## Multiple inheritance = inherit from more than one class c(A ,B)

## Multilevel inheritance = inherit from a parent from another parent C(B) <- B(A) <- A
```
class animal:
    def __init__(self, name):
        self.name = name

    def eat(self):
        print(f"{self.name} is eating")

    def sleep(self):
        print(f"{self.name} is sleeping")
class Prey(animal):
    def flee(self):
        print(f"{self.name} is fleeing")
class Predator(animal):
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
fish = Fish("Memo")

fish.sleep()
```


## super() =  Function used in child to call methods from a parent class (superclass).
- Allows you to extend the functionality of the inherited method

```
class Shape:
    def __init__(self, color, is_filled):
        self.color = color
        self.is_filled = is_filled

    def describe(self):
        print(f"It is {self.color} and {'filled' if self.is_filled else 'not filled'}")

class Circle(Shape):
    def __init__(self, color,is_filled, radius):
        super().__init__(color, is_filled)
        self.radius = radius

    def describe(self):
        super().describe()
        print(f"It is a circle with an area of {3.14 * self.radius * self.radius}cm^2")

class Square(Shape):
    def __init__(self, color, is_filled, width):
        super().__init__(color, is_filled)
        self.width = width

    def describe(self):
        super().describe()
        print(f"It is a square with an area of {self.width * self.width}cm^2")


class Triangle(Shape):
    def __init__(self, color, is_filled, width, height):
        super().__init__(color, is_filled)
        self.width = width
        self.height = height

    def describe(self):
        super().describe()
        print(f"It is a triangle with an area of {self.width * self.height / 2}cm^2")


circle = Circle(color="red", is_filled=True, radius=5)
square = Square(color="blue", is_filled=False, width=6)
triangle = Triangle(color="yellow", is_filled=True, width=7, height=8 )


circle.describe()
square.describe()
triangle.describe()

# print(triangle.color)
# print(triangle.is_filled)
# print(f"{triangle.width}cm")
# print(f"{triangle.height}cm")

```

## Polymorphism = Greek word that means to "have many forms or faces"
- poly = many
- morphe = form

- Two ways to achieve polymorphism
1. Inheritance = an object could be treated of the same as parents class
2. "Duck Typing" = Object must have necessary attributes/methods
```

from abc import ABC, abstractmethod

class Shape(ABC):

    @abstractmethod
    def area(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return  3.14 * self.radius * 2

class Square(Shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        return self.side ** 2

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

shapes = [Circle(4),  Square(5), Triangle(6,7), Pizza("Pepperoni", 15)]

for shape in shapes:
    print(f"{shape.area()}cm^2")
```

## Static methods = A method that belong to a class rather than any object from that class(instance)
- usually used for general utility functions

- Instance method = Best for operation of the class (object)
- Static methods = Best for utility function that do not need access to class data
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

employee1 = Employee("Eugune", "Manager" )
employee2 = Employee("Squidward", "Cashier")
employee3 = Employee("Spongebob", "Cook")


print(Employee.is_valid_position("Cook"))
print(employee1.get_info())
print(employee2.get_info())
print(employee3.get_info())
```
## Class methods = Allow operation related to the class itself
- Take (cls) as the first parameter, which represents the  class itself
```
class student:

    count = 0
    total_gpa = 0
    def __init__(self, name, gpa):
        self.name = name
        self.gpa = gpa
        student.count += 1
        student.total_gpa += gpa

    # Instance method
    def get_info(self):
        return f"{self.name} {self.gpa}"

    @classmethod
    def get_count(cls):
        return f"Total # of students: {cls.count}"

    @classmethod
    def get_average_gpa(cls):
        if cls.count == 0:
            return 0
        else:
            return f"Average gpa: {cls.total_gpa / cls.count:.2f}"

student1 = student("Spongebob", 3.2)
student2 = student("patrick", 2.2)
student3 = student("sandy", 3.9)


print(student.get_count())
print(student.get_average_gpa())
```

## Magic methods = Dunder methods (double underscore) __init__, __str__, __eq__
- They are automatically called by many of python's built-in operations.
- They allow developers to define or customize the behaviour of objects
from wsgiref.util import request_uri

```
class Book:

    def __init__(self, title, author, num_pages):
        self.title = title
        self.author = author
        self.num_pages = num_pages

    def __str__(self):
        return f"'{self.title}' by {self.author}"

    def __eq__(self, other):
        return self.title == other.title and self.author == other.author

    def __lt__(self, other):
        return  self.num_pages < other.num_pages

    def __gt__(self, other):
        return self.num_pages > other.num_pages

    def __add__(self, other):
        return f"{self.num_pages + other.num_pages} pages"

    def __contains__(self, keyword):
        return keyword in self.title or keyword in self.author

    def __getitem__(self, key):
        if key == 'title':
            return self.title
        elif key == "author":
            return self.author
        elif key == "num_pages":
            return self.num_pages
        else:
            return f"key '{key}' was not found"

book1 = Book("The Hobbit", "J.R.R. Tolkien", 310)
book2 = Book("Harry Potter and The Philosopher's Stone", "J.K Rowling", 223)
book3 = Book("The Lion, The Witch and the Wardrobe", "C.S. Lewis", 172)

# print(book3)
# print(book1 == book2)
# print("Lion" in book3)
# print(book2 < book3)
# print(book2 > book3)
# print(book2 + book3)
# print(book2['title'])
```

## @property = Decorator used to define a method as a property (it can be  accessed like an attribute)
- Benefits: add additional logic when read, write, or delete attributes
- Gives you getter, setter, and deleter method
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
        if new_width > 0:
            self._width = new_width
        else:
            print("Width must be greater than zero")

    @height.setter
    def height(self,  new_height):
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

rectangle.width = 6
rectangle.height = 5

del rectangle.height
del rectangle.width

# print(rectangle.width)
# print(rectangle.height)
```

## Decorator = A function that behavior of another function
- w/o modifying the base function
- Pass the base function as an argument to the decorator

```
def add_sprinkles(func):
    def wrapper(*args, **kwargs):
        print("you add sprinkles")
        func(*args, **kwargs)
    return wrapper

def add_fudge(func):
    def wrapper(*args, **kwargs):
        print("You add fudge")
        func(*args, **kwargs)
    return wrapper

@add_sprinkles
@add_fudge
def get_ice_cream(flavour):
    print(f"Here is your {flavour} ice cream")

get_ice_cream("chocolate")
```
## Exception = an event that interrupt the flow of a program
- (ZeroDivisionError, typeError, ValueError)
- 1.try, 2.except, 3.finally
```
try:
    number = int(input("Enter a number: "))
    print(1 / number)
except ZeroDivisionError:
    print("You can't divide by zero ")
except ValueError:
    print("Enter only numbers please!")
except Exception:
    print("Something went wrong!")
finally:
    print("Do some clean up here")
```

## Python file detection
```
import os

file_path = "C:/Users/binod/OneDrive/Desktop/New folder/myfile.txt"

if os.path.exists(file_path):
    print(f"The location {file_path} exists")
else:
    print("That location doesn't exist")
```

# Python writing files (.txt, .json, .csv)



- .txt
```
employees = ["spongebob", "patrick", "sandy", "squidward"]

file_path = "C:/Users/binod/PyCharmMiscProject/output.txt"

try:
    with open(file_path, "w") as file:
        for employee in employees:
            file.write(employee + "\n")
        print(f"txt file '{file_path}' was created")
except FileExistsError:
    print("That file already exists!")
```

- .json
```
import json
employee = {
    "name": "Spongebob",
    "age": "30",
    "job": "cook"
}
file_path = "C:/Users/binod/PyCharmMiscProject/output.txt"

try:
    with open(file_path, "w") as file:
        json.dump(employee, file, indent=4)
        print(f"json file '{file_path}' was created")
except FileExistsError:
    print("That file already exists!")
```
- .csv
```
import csv

employees = [["name", "age", "job"],
             ["spongebob", 30, "cook"],
             ["patrick", 37, "unemployed"],
             ["sandy", 27, "scientist"]]

file_path = "C:/Users/binod/PyCharmMiscProject/output.csv"

try:
    with open(file_path, "w", newline="") as file:
        writer = csv.writer(file)
        for row in employees:
            writer.writerow(row)
        print(f"csv file '{file_path}' was created")
except FileExistsError:
    print("That file already exists!")
```

## python reading files (.txt, .json, .csv)
- txt
```
file_path = "C:/Users/binod/PyCharmMiscProject/input.txt"

try:
    with open(file_path, "r") as file:
        content = file.read()
        print(content)
except FileExistsError:
    print("That file was not found")
except PermissionError:
    print("You do not have permission to read that file")
```
- json
```
import json

file_path = "C:/Users/binod/PyCharmMiscProject/output.txt"

try:
    with open(file_path, "r") as file:
        content = json.load(file)
        print(content["job"])
except FileExistsError:
    print("That file was not found")
except PermissionError:
    print("You do not have permission to read that file")

```
- csv
```
import csv

file_path = "C:/Users/binod/PyCharmMiscProject/output.csv"

try:
    with open(file_path, "r") as file:
        content = csv.reader(file)
        for line in content:
            print(line)
except FileExistsError:
    print("That file was not found")
except PermissionError:
    print("You do not have permission to read that file")
```
## Date and time in python
```
import datetime

date = datetime.date(2025, 1, 2)
today = datetime.date.today()

time = datetime.time(12,30,0)
now = datetime.datetime.now()

now = now.strftime("%H:%M:%S %m-%d-%y")

target_datetime = datetime.datetime(2020, 1, 2, 12, 30, 1)
current_datetime = datetime.datetime.now()

if target_datetime < current_datetime:
    print("Target date has passed")
else:
    print("Target date has not passed")
```

# Python alarm clock
```
import time
import datetime
import pygame

def set_alarm(alarm_time):
    print(f"Alarm set for {alarm_time}")
    sound_file = "stuff/crash.mp3"
    is_running = True

    while is_running:
        current_time = datetime.datetime.now().strftime("%H:%M:%S")
        print(current_time)

        if current_time == alarm_time:
            print("Wake up!!")

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

## Multithreading = Used to perform multiple tasks concurrently (multitasking)
- Good for I/O bound tasks like reading files or fetching data from APIs
- threading.Thread(target=my_function)
```
import threading
import time


def walk_dog(first, last):
    time.sleep(8)
    print(f"You finished walking {first} {last}")

def take_out_trash():
    time.sleep(2)
    print("You take out the trash")

def get_mail():
    time.sleep(4)
    print("You get the mail")
#
# walk_dog()
# take_out_trash()
# get_mail()

chore1 = threading.Thread(target=walk_dog, args=("scooby","Doo"))
chore1.start()

chore2 = threading.Thread(target=take_out_trash)
chore2.start()

chore3 = threading.Thread(target=get_mail)
chore3.start()

chore1.join()
chore2.join()
chore3.join()

print("All chores are complete!")
```

# How to connect to an API using python
```

import requests

base_url = "https://pokeapi.co/api/v2/"

def get_pokemon_info(name):
    url = f"{base_url}/pokemon/{name}"
    responce = requests.get(url)

    if responce.status_code == 200:
        pokemon_data = responce.json()
        return pokemon_data
    else:
        print(f"Failed to retrieve data {responce.status_code}")

pokemon_name = "pikachu"
pokemon_info = get_pokemon_info(pokemon_name)

if pokemon_info:
    print(f"Name: {pokemon_info["name"].capitalize()}")
    print(f"Id: {pokemon_info["id"]}")
    print(f"Height: {pokemon_info["height"]}")
    print(f"Weight: {pokemon_info["weight"]}")
```
