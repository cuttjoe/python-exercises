# Python Revision :dragon_face:
## Strings
1. Ask user for an 8 letter word 
    * and print only the 5th letter

a=""
while len(a)!=8:
	print("needs to be 8 letters")
	a=input("Give a letter with 8 letters")
print(a[4])
   
   *  Do the same as above but now print letters 3 to 5
   
a=""
while len(a)!=8:
	print("needs to be 8 letters")
	a=input("Give a letter with 8 letters")
print(a[2:5])

    *  Now print the word in reverse

a=""
while len(a)!=8:
	print("needs to be 8 letters")
	a=input("Give a letter with 8 letters")
print(a[::-1])

1. ask the user for two words and save them as strings. Now print as one string

a=input("enter a word")
b=input("enter another word")
print(a+b)

2. Ask the user to enter a word and write a procedure to count all the letter a's

a=input("enter a word")
print(a.count("a"))


3. Modify the procedure to count all the vowels in the word

a=input("enter a word")
print(a.count("a","e","i","o","u"))

## Lists
1. use lists to find all the unique letters in a sentence



2. Use lists to find all repeated words in a sentence
    * print out the number of times they are repeated
3. Replace all the vowels in a sentence with asterisks

