
Untitled5.ipynb
Untitled5.ipynb_

[ ]

data types in python


[ ]
x = 5
print(type(x))

x = "hello siet"
print(type(x))

x=20.5
print(type(x))

x=["apple","banana","cherry"]
print(type(x))

x=("apple","banana","cherry")
print(type(x))
x={"name":"meghana","age":19,"phno":1234567890}
print(type(x))
x=True
print(type(x))
x={"apple","banana","cherry"}
print(type(x))

#type conversion:conversion of a one data type to another data type
a=str(1)
print(type(a))
b=10
b=float(b)
print(type(b))
print(b)

y=int(2.8)
print(y)
<class 'int'>
<class 'str'>
<class 'float'>
<class 'list'>
<class 'tuple'>
<class 'dict'>
<class 'bool'>
<class 'set'>
<class 'str'>
<class 'float'>
10.0
2

[ ]
#conditional statement
a=33
b=200

if (a>b):
  print("a is greater than b")
elif a>b:
  print("b is less than a")
else:
  print("a is equal to b")


a is equal to b

[ ]
age=18
x = int("enter your age")

if age<18 :
  print("your not eligable for voteing")
elif age>18:
  print("you are eligable for voteing")
enter your age

[ ]
#random numbers
import random
y=int(random.randint(1,10))
while True:
  x=int(input("guess a number from 1 to 10:"))
  if x<y:
    print("too low!try again.")
  elif x>y:
    print("too high!try again.")
  else:
    print("you guessed it!")
    break #exit the loop after a correct guess
guess a number from 1 to 10:7
too high!try again.
guess a number from 1 to 10:6
too high!try again.
guess a number from 1 to 10:5
too high!try again.
guess a number from 1 to 10:4
too high!try again.
guess a number from 1 to 10:3
too high!try again.
guess a number from 1 to 10:2
you guessed it!

[ ]
# strings
a="meghana"
print(a[1])
for x in "banana":
  print(x)
print(len(a))
c="apple"
print(len(c))

e
b
a
n
a
n
a
7
5

[ ]
#text="the best things in life are free"
#print("expensive"not in text)
#string slicing

a="meghana"
print(a[1:7:2])
print(a[:7])
print(a[2:])
print(a[-5:-2])

# modifing strings


print(a.upper())
print(a.lower())
print(a.strip())
print(a.replace("a","A"))
print(a.split(","))
ehn
meghana
ghana
gha
MEGHANA
meghana
meghana
meghAnA
['meghana']

[ ]
"""#functions
def meghana():
  print ("hello meghana")
  print("how are you")
meghana()
"""
# arbitary arguments (*args)
def my_fun(fname,):
  print(fname+"ani")
my_fun("meghana")
my_fun("meghu")
my_fun("megha")

def my_fun(fname,lname):
  print(fname+""+lname)
my_fun("megha","l")

def my_fun(*kids):
  print("the youngest child is"+kids[2])
my_fun("meghana","chandu","yuktha")

#keyword arguments
def my_funn(students1,student2,student3):
  print("the youngest student is"+ student3)
my_funn("meghana","ani","amy")

# default parameters
def my_con(country = "india"):
  print("i am from" +country)
my_con("swedan")
my_con("usa")
my_con()
my_con("russia")
meghanaani
meghuani
meghaani
meghal
the youngest child isyuktha
the youngest student isamy
i am fromswedan
i am fromusa
i am fromindia
i am fromrussia

[ ]

def my_fun(x):
  return 5 * x
print(my_fun(1))
print(my_fun(2))
print(my_fun(3))
print(my_fun(4))
5
10
15
20

[ ]
def my_fun():
  pass

[ ]
# recursion:factorial program
def factorial(n):
  if n == 1:
    return 1
  else:
    return n * factorial(n-1)
factorial(5)
120

[ ]
def fibonacci(n):
  if n<=1:
    return n
  else:
    return fibonacci(n-1)+fibonacci(n-2)


term=int(input("enter the no of terms:"))

if term<=0:
  print("enter a positive integer")
else:
  print("fibonacci series:")
  for i in range(term):
    print(fibonacci(i))
enter the no of terms: 4
fibonacci series:
0
1
1
2

[ ]
# tuples:ordered unchangable allow duplicate values
"""thistuple =("apple","banana","cherry")
print(thistuple)
# tuples allows duplicate values
thistuple =("apple","banana","cherry","apple","cherry")
print(thistuple)
# finding the length of the tuple
print(len(thistuple))
# create a tuple with only one value
thistuple =("apple")
print(type(thistuple))
thistuple =("apple","banana","cherry")
print(thistuple[1])

# adding one tuple with an other
thistuple =("apple","banana","cherry")
sectuple=("orange",)
thistuple += sectuple #thistuple =thistuple +sectuple
print(thistuple)
# convert the tuple into a list and remove apple and convert into
thistuple =("apple","banana","cherry")
y =list(thistuple)
y.remove("apple")
thistuple =tuple(y)
print(thistuple)
#using the del keyword,through whichwe can delete the entire tuple
del thistuple
print(thistuple)

#looping in a tuple
thistuple=("apple","banana","cherry")
for i in thistuple:
  print(i)
  """
thistuple=("apple","banana","cherry")
i=0
while i<len(thistuple):
  print(thistuple[i])
  i=i1

tuple1=("a","b","c")
tuple2=(1,2,3)
apple
banana
cherry

[ ]
#length of a set
print(len(thisset))
#looping through the set
for i in thisset:
  print(i)

#checking weather a particular value  exists in a set or not

print("banana"in thisset)
print("banana"not in thisset)

grapes
papaya
apple
pineapple
cheery
False
True

[ ]
# adding from one set to another set
thisset={"apple","banana","cheery"}
otherset={"pineapple","papaya","grapes"}

thisset.update(otherset)
print(thisset)

#removing a particular element from a set

thisset.remove("banana")
print(thisset)

#using the clear method to empty the set

thisset.clear()
print(thisset)

# using the del keyword to delete the set entirely



{'grapes', 'banana', 'papaya', 'apple', 'pineapple', 'cheery'}
{'grapes', 'papaya', 'apple', 'pineapple', 'cheery'}

[ ]
# ROCK PAPER SCISSORS GAME
import random
def get_computer_choice():
  choices =["rock","paper","scissors"]
  return random.choice(choices)

def get_user_choice():
  user_choice =input("enter rock,paper,or scissors").lower()
  while user_choice not in ["rock","paper","scissors"]:
    print("Invalid choice! please do enter the choice again")
    user_choice= input("enter rock,paper or scissors").lower()
    return user_choice

def determine_winner(user_choice,computer_choice):
  if user_choice== computer_choice:
    return "its a tie!"

  if (user_choice=="rock" and computer_choice== "scissors")or \
     (user_choice=="scissors"and computer_choice== "paper")or \
     (user_choice=="paper" and computer_choice== "rock"):
     return "You win!"
  return "computer wins!"

def play_game():
  print("welcome to the ROCK PAPER SCISSORS GAME")
  user_choice=get_user_choice()
  computer_choice=get_computer_choice()

  print(f"You chose:{user_choice}")
  print("computer chose:{computer_choice}")

  result=determine_winner(user_choice,computer_choice)
  print(result)

play_game()

welcome to the ROCK PAPER SCISSORS GAME
enter rock,paper,or scissors ROCK
Invalid choice! please do enter the choice again
enter rock,paper or scissorsPAPER
You chose:paper
computer chose:{computer_choice}
You win!

[ ]
# algorithm
#Algorithms are procedures or formulas for solving problems
"""
#the order of complexity of algorithm
1:being the fastest
8:being the slowest

1:O(1)
2:O(logn)
3:O(n)
4:O(n^2)
5:O(n^3)
6:O(n^k)
7:O(2^n)
8:n!

#problem  no 1:calculate the sum  of  two number
1.start
2.take two numbers as input
3.add the two numbers
4.output the result
5.end


def add_numbers():
  a=int(input("enter the first number"))
  b=int(input("enter the second number"))
  return a+b
print(add_numbers())

def flow_division():
  a=int(input("enter the first number"))
  b=int(input("enter the second number"))
  return a//b
flow_division()
"""
enter the first number2
enter the second number3
5
enter the first number21
enter the second number5
4

[ ]
# algorithm to find the maximum value in the list
"""
1.start
2.take the no as list
3.finding the maxima value in the list
4.intilaze the first element to be maximum element
5.loop through the entire list
6.compare the each element which is the maximum with the next element in the list
7.if an element is found to be greater than the currenet
8.update the new maximum element
9.output the maximum value
10.end
"""
def find_max(numbers):
  max_value=numbers[0]
  for i in numbers:
    if i>max_value:
      max_value=i
  return max_value
print(find_max([3,7,14,1,2]))


14

[ ]
# algorithm for factorial program
"""
1.start
2.take the n value
3.if the number is 1 return 1
4.multiply the number by the factorial of (number-1)
5.end
"""
def fact(n):
  if n==1:
    return 1
  else:
    return n*fact(n-1)
print(fact(5))

# problem statement:print the fibonacci series of the no of terms entered
"""
1.start
2.take the n value
3.if n is less than or equal 1 then we return the value of n
4.else if the value is more than 1 then we do fibonnaci(n-1)+fibonnaci(n-2)
5.print the output
6.end

"""
def fib(n):
  if n<=1:
    return n
  else:
      return fib(n-1)+fib(n-2)

terms=int(input("enter the no of terms"))
if terms<=0:
  print("enter a pos value")
else:
  print("the fib series will be:")
  for i in range(terms):
    print(fib(i))
120
enter the no ofn terms4
the fib series will be:
0
1
1
2

[ ]
# pallindrome checking:
"""
1.start
2.take the input as a string
3.reverse the entered string
4.compare the existing string the reveresed string
5.if they are equal then we print that it is a pallindrome
6.end
"""
def is_pall(word):
  reversed_word=word[::-1]
  if word==reversed_word:
    return True
  else:
    return False
print(is_pall("madam"))
True

[ ]
# bubble sort:sorting of a given list using bubble ;e sort
"""
1.start
2.take the input as an array
3.consider 2 numbers and compare the first value with the adjacent value in the array
4.if the elements are in the worng order than swap them
5.repeat until no more swaps are needed
6.end
"""
def bubble_sort(arr):
  n=len(arr)
  for  i in range(n):
    for j in range(0,n-i-1):
      if arr[j]> arr[j+1]:
        arr[j],arr[j+1]=arr[j+1],arr[j]
  return arr
print(bubble_sort([7,14,1,16,21]))

[1, 7, 14, 16, 21]

[ ]
# linear search:linear search is a straight forward algorithm that checks
#each element in a list ,one by one until it finds the element we are looking for

def lin_search(arr,target):
  for i in range(len(arr)):
    if arr[i]==target:
      return i
  return-1
numbers=[10,20,30,40,50]
print(lin_search(numbers,40))


def lin_search(arr,target):
  for i in range(len(arr)):
    if arr[i]==target:
      return i #print(f"the element found at index  no {1})
    return -1
words=["mango","apple"]
print(lin_search(words,"apple"))
3
-1

[ ]

# binary search:it is a more efficient algorithm than liner search because it has a complexity of
#O(logn) unlike linear search which has a complexity of O(n) in binary search it repeatedly divides
#the searching interval in half if the target value is less than midpoint we go to the left side
#if it is more than the midpoint we go do to the right and find for the target value

def bin_search(arr,target):
  left=0
  right=len(arr)-1
  while left <=  right:
    mid=(left+right)//2
    if arr[mid]==target:
      return mid
    elif arr[mid]<target:
      left=mid
    else:
      right=mid-1
  return-1

numbers=[10,20,30,40,50]
print(bin_search(numbers,40))
3
Double-click (or enter) to edit


[ ]
import random
def love_calculate():
    print("welcome to love calculator")

    name1=input("enter the first name")
    name2=input("enter the second name")

    love_score = random.randint(1,100)
    print(f"the percentage of love between {name1} and {name2} is {love_score}%")

    love_calculate()

[ ]
ice_cream = [
    {"Flavours": "orange", "price": 10, "stock": 100},
    {"Flavours": "vanilla", "price": 18, "stock": 100},
    {"Flavours": "chocolate", "price": 25, "stock": 100},
    {"Flavours": "strawberry", "price": 15, "stock": 100},
]

def find_ice_cream(Flavours):
    for ice in ice_cream:
        if ice["Flavours"] == Flavours:
            return ice
    return None

def customer_choice():
    print("Welcome to Ani's Ice Cream Parlour")
    choice = input("Enter your choice (orange, vanilla, chocolate, strawberry): ").lower()
    while choice not in ["orange", "vanilla", "chocolate", "strawberry"]:
        print("Invalid choice! Please choose a valid flavour.")
        choice = input("Enter your choice (orange, vanilla, chocolate, strawberry): ").lower()
    return choice

def owner_choice():
    print("Hi! What flavour do you want to check?")
    choice = input("Enter a flavour (orange, vanilla, chocolate, strawberry): ").lower()
    while choice not in ["orange", "vanilla", "chocolate", "strawberry"]:
        print("Invalid choice! Please choose a valid flavour.")
        choice = input("Enter a flavour (orange, vanilla, chocolate, strawberry): ").lower()
    return choice

def show_stock():
    print("Current stock levels:")
    for ice in ice_cream:
        print(f"{ice['Flavours'].capitalize()}: {ice['stock']} units")

while True:
    role = input("Are you a customer or owner? (Enter 'customer', 'owner', or 'exit' to quit): ").lower()
    if role == "customer":
        Flavours = customer_choice()
        selected_ice_cream = find_ice_cream(Flavours)
        if selected_ice_cream and selected_ice_cream["stock"] > 0:
            selected_ice_cream["stock"] -= 1
            print(f"Enjoy your {Flavours} ice cream! Remaining stock: {selected_ice_cream['stock']}")
        else:
            print(f"Sorry, {Flavours} ice cream is out of stock!")
    elif role == "owner":
        Flavours = owner_choice()
        selected_ice_cream = find_ice_cream(Flavours)
        if selected_ice_cream:
            print(f"The remaining stock of {Flavours} ice cream is {selected_ice_cream['stock']}")
    elif role == "exit":
        print("Thank you for visiting! Have a great day!")
        break
    else:
        print("Invalid role! Please enter 'customer', 'owner', or 'exit'.")

    show_stock()
Invalid role! Please enter 'customer', 'owner', or 'exit'.
Current stock levels:
Orange: 100 units
Vanilla: 100 units
Chocolate: 100 units
Strawberry: 100 units
Invalid role! Please enter 'customer', 'owner', or 'exit'.
Current stock levels:
Orange: 100 units
Vanilla: 100 units
Chocolate: 100 units
Strawberry: 100 units
Invalid role! Please enter 'customer', 'owner', or 'exit'.
Current stock levels:
Orange: 100 units
Vanilla: 100 units
Chocolate: 100 units
Strawberry: 100 units
Invalid role! Please enter 'customer', 'owner', or 'exit'.
Current stock levels:
Orange: 100 units
Vanilla: 100 units
Chocolate: 100 units
Strawberry: 100 units

[ ]
# binary search for transaction by Amount
def search_by_amount(target_amount):
  transcations.sort(key=lambda x:x["amount"])
  left = 0

  right = len(transactions)  - 1
  while left <= right:
      mid = (left + right)  //2
      if transactions[mid]["amount"]==target_amount:
        return transactions[mid]
      elif transactions[mid]["amount"]<target_amount:
        left=mid
      else:
        right=mid-1
  return "transactions not found"
print(search_by_amount(50.0))

#adding a new expense
def add_expense(date,amount,description):
  new_transaction={"date":date,"amount":amount,"description":description}
  transaction.append(new_transactions)
  return"expense added sucessfully!"


#checking amount by description
def total_spent_by_description(description):
  total_spent=sum(transaction["amount"] for transaction in transactions if transactions if transaction["description"].lower()==description.lower())
  if total_spent>0:
    return {"description":description, "total_spent":total_spent}
  else:
     return "no expenses were found for this description in the transactions"
# displaying all of the expenses

def display_all_expenses():
  if transactions:
    return transcations
  else:
    return "no transactions available"




[ ]
!pip install gradio
import gradio as gr
#binary search for transaction by amount
transactions=[
    {"date":"2024-08-01","amount":50.0,"description":"groceries"},
    {"date":"2024-08-02","amount":500.0,"description":"ring"},
    {"date":"2024-08-03","amount":100.0,"description":"electricity bill"},
    {"date":"2024-08-04","amount":200.0,"description":"new shoes"}
]

def search_by_date(target_date):
  for transaction in transactions:
    if transaction["date"]==target_date:
      return transaction
  return "transaction not found"

def search_by_amount(target_amount):
  transactions.sort(key=lambda x:x["amount"])
  left = 0

  right = len(transactions)  - 1
  while left <= right:
      mid = (left + right)  //2
      if transactions[mid]["amount"]==target_amount:
        return transactions[mid]
      elif transactions[mid]["amount"]<target_amount:
        left=mid
      else:
        right=mid-1
  return "transactions not found"
print(search_by_amount(50.0))

#adding a new expense
def add_expense(date,amount,description):
  new_transaction={"date":date,"amount":amount,"description":description}
  transactions.append(new_transaction)
  return"expense added sucessfully!"


#checking amount by description
def total_spent_by_description(description):
  total_spent=sum(transaction["amount"] for transaction in transactions if transaction["description"].lower()==description.lower())
  if total_spent>0:
    return {"description":description, "total_spent":total_spent}
  else:
     return "no expenses were found for this description in the transactions"
# displaying all of the expenses

def display_all_expenses():
  if transactions:
    return transactions
  else:
    return "no transaction available"

#building a gradio interface for our expenses tracker application
with gr.Blocks() as demo:
  gr.Markdown("# expense tracker")





  with gr.Tab("search By Date:"):
    date_input=gr.Textbox(label="enter date(YYY-MM-DD)")
    #json is javascript object notation which is the text base format of storing strings
    date_output=gr.JSON(label="result")
    gr.Button("search").click(fn=search_by_date,inputs=date_input,outputs=date_output)

  with gr.Tab("search By amount"):
    amount_input=gr.Number(label="enter amount")
    #json is javascript object notation which is the text base format of storing strings
    amount_output=gr.JSON(label="result")
    gr.Button("search").click(fn=search_by_amount,inputs=amount_input,outputs=date_output)

  with gr.Tab("add a new expense"):
    date_input=gr.Textbox(label="enter Date(YYYY-MM-DD)")
    amount_input=gr.Number(label="enter amount")
    description_input=gr.Textbox(label="enter the description")
    add_output=gr.Textbox(label="status")
    gr.Button("ADD EXPENSE").click(fn=add_expense,inputs=[date_input,amount_input,description_input],outputs=add_output)

  with gr.Tab("Display All Expenses"):
    all_expenses_output = gr.JSON(label="All Expenses")
    gr.Button("Show All Expenses").click(fn=display_all_expenses,outputs=all_expenses_output)

demo.launch()




[ ]
from ctypes import sizeof
# pizzabilling system
class Pizza:
  def_init_(self,size,toppings):
    self.size=size
    self.toppings=toppings

  def cal_price(self):
    base_price=0
    if self.size== "small":
      base_price=10
    elif
Colab paid products - Cancel contracts here
- 👋 Hi, I’m @meghanasmitha
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
meghanasmitha/meghanasmitha is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
