# ECE-2112-PA1

Made and Submitted by Charles Steven H. Ang | 2ECE-D

The content of this repository is the code for the First ECE2112 Experiment (PA1) AY2026-2027. This Experiment introduces Python programming by presenting 3 programming problems.

A. WORD ROTATION PROBLEM
Create a function named rotate_word() that accepts a non-empty string. Move the first character
of the string to the end while keeping all remaining characters in their original order. Preserve the
capitalization of every character.

  **The Following Methods/Functions were used:**
'''python
def rotate_word(word: str) -> str:
 
    if not isinstance(word, str) or not word.strip():
        raise ValueError("Argument must be a non-empty string.")
'''




The problem stated that the function "rotate_word()" must accept a non-empty string, which is why isinstance(), ".strip", and "raise" were used. "isinstance()" checks if a variable belongs within a certain data type, which in this case, is (string). The ".strip" was used to clear up the "spaces" input by the user, so it can be checked with a logical operator (or not), therefore making the function "rotate_word()"only accept non-empty string type variables.

The main part of the function "rotate_word()" used "len()" to identify the number of characters in the word input. To stop the function from breaking, it will return the word input if the length of the word is <= 1. This means the user used the function on a single letter, and the output will be the same letter.

When the user inputs a word that is > 1, then the function would return the last character in front using "word[-1]", then the middle characters of the word untouched using "word[1:-1]," and lastly the first character at the end of the word. This works by using Python indexing, where [-1] is the last character of a word, [1] is the second character, and [0] or [-(total number of characters)] is the first character. Think of it this way, positive-upwards goes from left to right, negative-downwards goes from right to left, and [0] is the start from left to right, and [-(total number of characters)] is the end from right to left.

What the function returns is the last character in front, keeping the middle untouched by using a slicing operator ":" inside "word[1:-1]", and the first character at the end. <br>
<br>

B. USERNAME BUILDER PROBLEM
Create a function named make username() that accepts two strings: first name and last name.

C. BOOKEND SWAP PROBLEM
Create a function named swap bookends() that accepts a list containing at least two elements.


To see the main Python program for Experiment 1, click this link: _________________________________________ and download it, open it in Jupyter Notebook, then run all cells.

Thank you for reading!!

**README FILE VERSION HISTORY**\
August 20, 2026 - Inputted the initial base for the README file.
August 21 2026 - Added descriptions of the functions and methods to Problems A and B



