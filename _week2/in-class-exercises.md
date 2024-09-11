# In-Class Exercises

Wednesday, Sept 11, 2024


Guidelines for pair-work:

- The important thing is not to finish first, but to work together. 
- Take turns with **each step** of the exercise.
- If you know the answer, give your partner a chance to work it out for themselves.
- If neither of you know the answer, look back over the materials and ask Prof. Eckert  

For each other exercises below, **record the command that you input.**

## Exercise 1: Words as Things in Gertrude Stein's "Matisse" and "Picasso"

- Open [the command line cheat sheet](https://github.com/sceckert/Data-and-Culture-Fall-2024/blob/main/_week2/command-line-cheat-sheet.md)
- Make a directory called "my_texts"
- In a web-browser, navigate to [the files for this week](https://github.com/sceckert/Data-and-Culture-Fall-2024/blob/main/_week2). I've created two text files of the "Matisse" and "Picasso" pieces, with each sentence on a new line. First, click on and open "stein-matisse.txt." Click on the button in the upper right hand corner that says "RAW". Then, right click and save the page into the directory you just created. Do the same thing for "stein-picasso.txt"
- In the terminal, navigate to the directory where you saved the two text files. Verify that you have both the text files there. 
- Using the commands we've learned, figure out the number of words in each text. Which one is longer?
- Try to look at just the first 5 lines and the last five lines of "stein-matisse.txt." Repeat for "stein-picasso.txt."
- Then, search for and count all instances of the word "some" in "stein-matisse.txt."
- Then, search for all instances of the word "some", in "stein-matisse.txt.**ignoring case**. 
- Do the same thing as above for the words "something", "expressing", and "working."
- Repeat the search for "some", "something", "working" and expressing for "stein-picasso.txt"
- What did you notice? 
- Try searching for other words or patterns. Talk about your findings. What was it like to read in this way?

---
>✨***HINT***✨:
 Remember to include the path to the directory. If you're in a directory that contains a subdirectory (a directory within a directory) with text files you would like to perform commands on, you don't have to move into the directory to perform commands on the text files -- just include the path in your command:

> Macs: `grep "search term" directoryname/filename.txt` or `grep "search term" directoryname/*` if you want to use a wildcard to search *all* the files in that directory

>Windows: ` gc .\directoryname\filename.txt | Select-String -Pattern "search term"` or  `gc .\directoryname\* | Select-String -Pattern "search term"` if you want to use a wildcard to search all the files in that directory 
`
---

## Exercise 2: Imagining "America," Part 1

Download and unzip the **revised** corpus of [US Inaugural Addresses](https://github.com/sceckert/Data-and-Culture-Fall-2024/blob/main/_datasets/US_Inaugural_Addresses.zip?raw=true) and complete the following exercises on the command line (*NOTE: you must use this folder, not the previously shared link*)

1. Count the number of words in Biden's recent inaugural address
2. Search inside Biden's inaugural address for all instances of the term "America"  and display the results with the corresponding line numbers and your search term highlighted
3. Now, search for the term "America" in Biden's address and return the number of lines the term appears on.
 
## Exercise 3: Imagining "America," Part 2

1. Use a single command to search inside the folder of ["US_Inaugural_Addresses"](https://github.com/sceckert/Data-and-Culture-Fall-2024/blob/main/_datasets/US_Inaugural_Addresses.zip?raw=true) [Remember that you'll have to unzip this file first] for **all** instances of the term "America" in all 59 speeches and print the results with the search term highlighted
2. Output the results of your keyword search to a text file
3. Make a second search, but this time include 1 additional line of context **before** and **after** the line that your term appears in.
4. Generate a second text file that contains the output of your new keyword search above.


*If you finish early, practice using some of the commands you just learned on this corpus!* 