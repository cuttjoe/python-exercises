# Python Revision 1
## Mathematical operations  
/ + - % // %
1. calculate the hypotenuse of a right angle triangle with sides 6 and 7 cm
a=6
b=7
c=a**2+b**2
print (c**0.5)
1. what does 
```python
print(17//5)
```
get you and why?  
it gets you 3
because 17 can be devided by 5, 3 times

3. Print all numbers below 75 dividable by 7

for i in range (75):
	if i%7==0:
		print (i)
		
1. Now do it without using modular division

a=7 
while a<=70:
	print (a)
	a=a+7

## Input /output
5. Ask user for a number and a name  
    Now print the name with as many spaces between the letters  
    Also print the name as may times as the number
    a=str(input("enter a name"))
    
b=int(input("enter a number"))
for i in range(b):
	c="\t"
	d=" "
for j in a:
	c=c+j+" "*b
print (c)
for i in range (b):
	print (a)
	
5. Ask user for a name and print name one letter at a time (separate lines)  
	Now print the letters diagonally across the page one letter at a time (separate lines)
	
a=str(input("enter a name"))
for i in range (len(a)):
	print (" "*i,a[i])
	
6. Figure out how to print this pattern below with and without using a loop (its just a formatting trick)

list=[1,3,5,7,9]
for i in list:
	print ('{:^12}'.format(i*"*"))
	
print('{:^12}'.format(1*"*"))
print('{:^12}'.format(3*"*"))
print('{:^12}'.format(5*"*"))
print('{:^12}'.format(7*"*"))
print('{:^12}'.format(9*"*"))
```
     *
    ***
   *****
  *******
 *********
```
![geek joke](http://i.imgur.com/KGrV41o.png)
