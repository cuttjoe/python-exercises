# Python Revision 1
## Mathematical operations  
/ + - % // %
1. calculate the hypotenuse of a right angle triangle with sides 6 and 7 cm

a=6**2
b=7**2
c=(a+b)**0.5
print(c)


1. what does 
```python
print(17//5)
```
get you and why?  

An answer of 3 is given.
 The operation // is a form of division. 5 can evenly divide into 17 a total of 3 times, thus the answer 3 is printed.

3. Print all numbers below 75 dividable by 7

for i in range(1,75):
	if i%7==0:
		print (i)

1. Now do it without using modular division


for i in range (1,75):
	if i/7==i//7:
		print(i)

## Input /output
5. Ask user for a number and a name  
    Now print the name with as many spaces between the letters  
    
list=[]
name=input("What is your name?")
number=int(input("What is your number?"))
x=len(name)
for i in range(x):
	list.append(name[i])
	list.append(" "*x)
print(list)
 
    Also print the name as may times as the number
    
    
name=input("What is your name?")
number=int(input("What is your number?"))
print(name*number)


5. Ask user for a name and print name one letter at a time (separate lines)  


Name=input("Please enter your first name: ")
for letter in Name:
     print(letter)


	Now print the letters diagonally across the page one letter at a time (separate lines)
	
	
name=input("What is your name?")
for i in range(len(name)):
	print(" "*i, name[i])
	
	
6. Figure out how to print this pattern below with and without using a loop (its just a formatting trick)  
```
     *
    ***
   *****
  *******
 *********
```

With Loop:

list=[1,3,5,7,9]
for i in list:
	print('{:^12}'.format(i*"*"))

Without Loop:

print('{:^12}'.format(1*"*"))
print('{:^12}'.format(3*"*"))
print('{:^12}'.format(5*"*"))
print('{:^12}'.format(7*"*"))
print('{:^12}'.format(9*"*"))


![geek joke](http://i.imgur.com/KGrV41o.png)
