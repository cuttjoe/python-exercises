# Python Revision :dragon_face:
## Strings
1. Ask user for an 8 letter word 
    * and print only the 5th letter
    *  Do the same as above but now print letters 3 to 5
    *  Now print the word in reverse
    
a=input("enter an 8 letter word")
print (a[4])
print (a[2:5])
print (a[::-1])


1. ask the user for two words and save them as strings. Now print as one string

a=str(input("enter one word"))
b=str(input("enter another word"))
print(''.join((a,b)))

2. Ask the user to enter a word and write a procedure to count all the letter a's

a=input("enter a word")
b=a.count("a")
print(b)

3. Modify the procedure to count all the vowels in the word

a=input("enter a word")
b=a.count("a")
print(b)
b=a.count("e")
print(b)
b=a.count("i")
print(b)
b=a.count("o")
print(b)
b=a.count("u")
print(b)

## Lists
1. use lists to find all the unique letters in a sentence
2. Use lists to find all repeated words in a sentence
    * print out the number of times they are repeated
3. Replace all the vowels in a sentence with asterisks

![Smile](http://www.kdnuggets.com/images/cartoon-deep-learning-2nd-place-coffeemaker.jpg)
