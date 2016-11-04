# Python Revision :dragon_face:
## Strings
1. Ask user for an 8 letter word 
    * and print only the 5th letter
    
a=input("What is your 8 letter word?")
x=len(a)
if x>8:
	print("Your word is greater than 8 letters long")
elif x<8:
	print("Your word is less than 8 letters long.")
elif x==8:
	fifth_letter = a[4]
	print("The fifth letter of the word is ",fifth_letter)
	
 
    *  Do the same as above but now print letters 3 to 5
    
a=input("What is your 3-5 letter word?")
x=len(a)
if x>5:
	print("Your word is greater than 5 letters long")
elif x<3:
	print("Your word is less than 3 letters long.")
elif x==3 or x==4:
	print("The word you have chosen is within the required word count,however it does not contain a fifth letter.")
elif x==5:
	fifth_letter = a[4]
	print(fifth_letter)  

    
    *  Now print the word in reverse
    
a=input("What is your 8 letter word?")
x=len(a)
if x>8:
	print("Your word is greater than 8 letters long")
elif x<8:
	print("Your word is less than 8 letters long.")
elif x==8:
	print(a, "in reverse is ", a[::-1])
   
	
1. ask the user for two words and save them as strings. Now print as one string

a=str(input("Enter one word"))
b=str(input("Enter another word"))
print(''.join((a, b)))

OR

a=str(input("Enter one word"))
b=str(input("Enter another word"))
print(a+b)

2. Ask the user to enter a word and write a procedure to count all the letter a

word=input("Enter a word")
wc=word.count("a")
print("There is ", wc," a's in the word")

3. Modify the procedure to count all the vowels in the word

word=input("Enter a word")
wc=word.count("a")
print("There is ", wc," a'/s in the word")
wc=word.count("e")
print("There is ", wc," e'/s in the word")
wc=word.count("i")
print("There is ", wc," i'/s in the word")
wc=word.count("o")
print("There is ", wc," o'/s in the word")
wc=word.count("u")
print("There is ", wc," u'/s in the word")


## Lists
1. use lists to find all the unique letters in a sentence
2. Use lists to find all repeated words in a sentence
    * print out the number of times they are repeated
3. Replace all the vowels in a sentence with asterisks

![Smile](http://www.kdnuggets.com/images/cartoon-deep-learning-2nd-place-coffeemaker.jpg)
