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
  return(l)
print(throw(10))

#Oceanverse37
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
                
  
