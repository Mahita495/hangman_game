# Hangman Game  

It is word guessing game where the player has to guess the word by checking letter by letter. If he guesses wrong letter, he loses a life.  
For each correct guess, the word will be filled. Th player has fixed no of lives to guess the word.  

Procedure:  

Initially take some random words and store in a list  
One random word will be chosen and given as blank for the user to find.  
User must find the correct word letter by letter to guess the given blank word. If the user reaches no of failed attempts, he loses else, he wins  
Consider list of hangman objects to keep track of failed attempts  
Methods to include in game:  
Initialise no of failed attempts as 0, and list of blanks to track the word progress    
1.	Word to guess: a list of blanks(word progress) with length of chosen word will be displayed   

2.	Find indexes: In the chosen word, we need to find the guessed letter’s index   

3.	Failed attempts: if guessed letter not in chosen word, count of failed attempts increases,  


4.	Invalid letter: If entered value is a digit or word lo length>1, then print as invalid letter  

5.	Game status: For each failed attempt, objects of hangman will be printed to show that lives are decreasing  

6.	Update progress: If guessed letter matches any letter of chosen word, update the index of blank list (word progress) and insert the letter  

7.	User input: Take user input  

8.	Game play: Until the user finishes all his failed attempts, he can guess the word  

First print game status and game progress  
Print the guessed letter   
First Check if letter is valid or not   
Next check if letter is already present in  word progress  
If letter in chosen word, find the index, update progress in blank list  
Check the count of remaining blanks, If count is 0 – User won, print the word and quit  
	Else, increment the failed attempts  
