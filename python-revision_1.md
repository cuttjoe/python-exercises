# Python Revision 1
## Mathematical operations  
/ + - % // %
1. calculate the hypotenuse of a right angle triangle with sides 6 and 7 cm

a=6
b=7
c=a**2+b**2
d=c**0.5
print("the hypotenuse is", d)

1. what does 
```python
print(17//5)
```get you and why?  
3, as 3 is the max amount of times 5 goes into 17 without a remainder


3. Print all numbers below 75 dividable by 7
for i in range(0,75):
	a=i%7
	if a==0:
		print(i)
1. Now do it without using modular division

for i in range(0,75):
	if i/7==i//7:
		print(i)

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
