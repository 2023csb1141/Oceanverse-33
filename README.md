# Oceanverse-33
# program to make a function called add that takes two numbers as arguments and returns their sum

def sum(a,b) :
  return(a+b)

print(sum(22,57)

# Oceanverse-34
# Program to make a function that takes an integer n and returns the factorial of n
def factorial(n) :
  k=1
  for i in range(1,n+1) :
    k*=i
  return(k)
print(factorial(7))

# Oceanverse-35
# Program to  make a function called fibonacci that takes an integer n and returns the n-th number in the Fibonacci sequence

def fibonacci(n) :
  l=[1,1]
  for i in range(2,n) :
    l.append(l[i-2]+l[i-1])
  return(l[n-1])
print(fibonacci(11))

# Oceanverse-36
# Program to write a function which simulates the process of throwing n identical balls into n bins. What is the maximum across the buckets? Write a short report on the output of your code.
import random
def throw(n) :
  l=[]
  for i in range(n) :
    l.append([])
  for i in range(n) :
    l[random.randint(0,n-1)].append(1)
  a=0
  for i in range(len(l)) :
  if len(l[i])>a :
    a= len(l[i])
  return(l,a)
print(throw(10))

#Oceanverse-37
# Program to make function which simulates the throwing of n balls in n identical bins till all bins are empty
import random
def throw(n) :
    l=[]
    for i in range(n) :
        l.append([])
    j=0
    while j<len(l)-1 :
        if l[j]==[] :
            l[random.randint(0,n-1)].append(1)
        else :
            j+=1
    return(l)
print(throw(30))
                
  
#Oceanverse-38
# Program to make a function which returns true if number n is even and false if not

n= eval(input("Enter a number to know if its even- "))
def is_even(n) :
    if n%2==0 :
        return(True)
    else :
        return(False)
print(is_even(n))

#Oceanverse-39
# Program to make a function to take radius of a circle and return its area

k= eval(input("Enter the radiu sof the circle- "))
def circle_area(r) :
    ar= (22*r*r)/7
    return(ar)
print(circle_area(k))

#Oceanverse-40
# Program to define a function that displays the spiral: RULLDDRRRUUULLLL… and so on. It should keep displaying until it has displayed 1,000,000 Letters in this pattern

def spiral(n) :                # Defining a function called spiral
    i=1
    z=""                       # Defining an empty string which will hold our spiral direction values
    a=len(z)                   # Defining a variable which will be the length of our string
    while a<n :                # Setting a while loop to keep adding direction values to our string till it has reached its limit of just greater than n letters
        if i%2!=0 :            # Putting condition to add R, U in every alternate loop
            z=z+("R"*i)
            z=z+("U"*i)
        if i%2==0 :            # Putting condition to add L, D in every alternate loop
            z=z+("L"*i)
            z=z+("D"*i) 
        a=len(z)               # Changing the value of a to the new length of string z in each iteration
        i+=1                   # Incrementing value of i (which runs our loop) in every iteration 
    return(z[:n])              # Returning the string with all values of the direction in our spiral upto n letters only

print(spiral(1000000))         # Printing our spiral upto 1 million letters


#Oceanverse-41
# Program to make a function that takes two strings and concatenates them with a space in between

def concatenate(a,b) :
    return(a+" "+b)

print(concatenate("Hello","World"))

                                                                                                                                                                                      
#Oceanverse-42
# Program to make a function that takes a list of numbers and finds the maximum of them

import random
l=[]
for i in range(20) :
    l.append(random.randint(1,40))
print(l)

def find_max(l) :
    k=l[0]
    for i in range(1,len(l)-1) :
        if l[i]>k :
            k=l[i]
    return(k)

print(find_max(l))
