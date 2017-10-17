# Python Revision :dragon_face:
## Strings
1. Ask user for an 8 letter word 
    * and print only the 5th letter
    *  Do the same as above but now print letters 3 to 5
    *  Now print the word in reverse
1. ask the user for two words and save them as strings. Now print as one string
2. Ask the user to enter a word and write a procedure to count all the letter a's
3. Modify the procedure to count all the vowels in the word
4. Create a passsword generator using a random combination of letters numbers and symbols
5. Create a user login name creator. Ask user for name, and surname; use the first 4 letters of the name and first 3 letters  
of the surname plus dm2017 to create a new username. Print username out.

## Lists
1. use lists to find all the unique letters in a sentence
2. Use lists to find all repeated words in a sentence
    * print out the number of times they are repeated
3. Replace all the vowels in a sentence with asterisks
4. Simulate a text compression algorithm by extraction the 3 most common words in a sentence and replacing them with numbers.


![Smile](http://www.kdnuggets.com/images/cartoon-deep-learning-2nd-place-coffeemaker.jpg)

Strings:
import sys
print("Question 1:")
done1=0
print("")
print("")
while done1==0:
	word=input("Input> Enter a 8 letter word")
	print("")
	if len(word)==8:
		print("Console> 8 letter word detected!")
		print("")
		print("Console> The 5th letter is", word[4:5])
		print("")
		print("Console> Letters 3 to 5 are", word[2:5])
		print("")
		print("Console> The reverse of the string enterd is", word[::-1])
		print("")
		done1=1
	else:
		print("Console> The number in which you entered is not a 8 letter word")
		print("")
	if any(ch.isdigit() for ch in word):
		print ("Console>", (word),"contains a digit! Letters only!")
		print("")
print("")
print("")
print("Question 2:")
print("")
print("")
done2=0
word1complete=0
while done2==0:
	while word1complete==0:
		string1=input("Input> Enter a word")
		print("")
		if (' ' in string1)==True:
			print("Console> That is not a word! That is a sentence!")
			print("")
		if any(ch.isdigit() for ch in string1):
			print ("Console>", (string1),"contains a digit! Letters only!")
			print("")
		if (' ' in string1)==False:
			if any(ch.isdigit() for ch in string1):
				a=1
			else:
				word1complete=1
	while word1complete==1:
		string2=input("Input> Enter a second word")
		print("")
		if (' ' in string2)==True:
			print("Console> That is not a word! That is a sentence!")
			print("")
		if any(ch.isdigit() for ch in string2):
			print ("Console>", (string2),"contains a digit! Letters only!")
			print("")
		if (' ' in string2)==False:
			if any(ch.isdigit() for ch in string2):
				a=1
			else:
				word1complete=3
				print("Console> Both word combined is:", string1+string2)
				print("")
				done2=1
print("")
print("")
print("Question 3:")
print("")
print("")
done3=0
while done3==0:
	aword=input("Input> Enter a word")
	print("")
	if any(ch.isdigit() for ch in aword):
		print ("Console>", (aword),"contains a digit! Letters only!")
		print("")
	if (' ' in aword)==False:
		if any(ch.isdigit() for ch in aword):
			a=1
		else:
			from collections import Counter
			counter = Counter(aword)
			print("Console> The number of a's are:", counter['a'])
			print("")
			print("")
			print("Question 4:")
			print("")
			print("")
			vowels=(counter['a']+counter['e']+counter['i']+counter['o']+counter['u']+counter['A']+counter['E']+counter['I']+counter['O']+counter['U'])
			print("Console> Total vowels are:", (vowels))
			sys.exit()s




Lists:
from collections import Counter
import re
print("Question 1 and 2:")
print("")
input=input("Make a list:")
list1=[]
for i in range(len(input)):
	list1.append(input[i])
list2=[]
for i in range(len(list1)):
	if any([list1[i] in list2 for item in list1]):
		counter = Counter(list1)
		common=(counter[(list1[i])])
		print(list1[i], "is common", (counter[(list1[i])]), "times.")
		list2.remove((list1[i]))
	else:
		list2.append(list1[i])
print("Unique letters are:", (list2))
vowels = ('a', 'e', 'i', 'o', 'u')
listvowel=[]
print("")
print("Question 3")
print("")
for i in range(len(input)):
	listvowel.append(input[i])
print(re.sub("a|e|i|o|u", "*", input))






