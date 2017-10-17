# Python Revision 1
## Mathematical operations  
/ + - % // %
1. calculate the hypotenuse of a right angle triangle with sides 6 and 7 cm
1. what does 
```python
print(17//5)
```
get you and why?  

3. Print all numbers below 75 dividable by 7
1. Now do it without using modular division

## Input /output
5. Ask user for a number and a name  
    Now print the name with as many spaces between the letters  
    Also print the name as may times as the number
5. Ask user for a name and print name one letter at a time (separate lines)  
	Now print the letters diagonally across the page one letter at a time (separate lines)
6. Figure out how to print this pattern below with and without using a loop (its just a formatting trick)  
```
     *
    ***
   *****
  *******
 *********
```
![geek joke](http://i.imgur.com/KGrV41o.png)

PYTHON REVISION 1


a=6
b=7
c=a*a+b*b
print (c)
d=(c ** 0.5)
print (d)


a=17
b=5
c=a//b
print(c)


for i in range(1,76):
	if i%7 == 0:
		print(i)



name=input("Enter a name")
name2=""
number=int(input("Enter a number"))
for i in name:
	name2=name2+i+number*" "
print(name2)

name=input("Enter a name")
for i in range(3):
	print("\t"*i+name[i])

