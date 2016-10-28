# Python Revision 1
## Mathematical operations  
/ + - % // %
1. calculate the hypotenuse of a right angle triangle with sides 6 and 7 cm

a=6
b=7
c=6**2
d=7**2
e=c+d
f=e**0.5
print (f)

1. what does 
```python
print(17//5)
```
get you and why?  
print(17//5) gives you 3 because the //5 calculates the amount of times 5 goes into 17 completly

3. Print all numbers below 75 dividable by 7

list=[]
a=75//7
for i in range(1,a+1):
	b=7*i
	list.append(b)
print(list)

1. Now do it without using modular division

list=[]
for i in range (1,75):
	if i%7==0:
		list.append(i)
print(list)


## Input /output
5. Ask user for a number and a name  
    Now print the name with as many spaces between the letters  
    Also print the name as may times as the number
    a=int(input("enter a number"))

b=input("enter a name")
list=[]
count=0
for i in range (0,(len(b))):
	list.append(b[i])
	for i in range(0,(len(b))):
		list.append(" ")
c=''.join(list)
for i in range(a):
	count=count+1
	print(c)

	
5. Ask user for a name and print name one letter at a time (separate lines)  

a=input("give me a name")
b=list(a)
for i in range(len(a)):
	print(b[i])

	Now print the letters diagonally across the page one letter at a time (separate lines)

a=input("give me a name")
b=list(a)
for i in range(len(a)):
	print((" ")*i,b[i])



6. Figure out how to print this pattern below with and without using a loop (its just a formatting trick)  
```
     *
    ***
   *****
  *******
 *********
```
for i in range(1,11,2):
	a=i*"*"
	print('{:^12}'.format(a))
