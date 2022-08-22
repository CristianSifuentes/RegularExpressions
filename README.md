# RegularExpressions



   * [Introduction to Regular Expressions
](#introduction-to-regular-expressions)
      * [Everything you will learn about regular expressions](#everything-you-will-learn-about-regular-expressions)
      * [What are regular expressions?](#what-are-regular-expressions)
      * [Applications of regular expressions](#applications-of-regular-expressions)
       * [Introduction to the regular expression language](#introduction-to-the-regular-expression-language)      
   * [The language: characters, operators, and constructions
](#the-language-characters-operators-and-constructions
)  
      * [The character (.)](#the-character.) 
      * [Predefined and built classes
](#predefined-and-built-classes) 
      * [The delimiters: +, *, ?
](#the-delimiters)
      * [Counters {1,4}
](#counters)
      * [The case of (?) as a delimiter
](#the-case-of-as-a-delimiter)
      * [Not (^), its use and its dangers
](#not-its-use-and-its-dangers)
      * [Challenge: Filtering out letters in phone numbers using negations
](#challenge-filtering-out-letters-in-phone-numbers-using-negations)
      * [Beginning (^) and end of line ($)
](#beginning-and-end-of-line)


   * [Practical use of Regular Expressions
](#practical-use-of-regular-expressions
)   
      * [Logs
](#logs) 
      * [Phone
](#phone) 
      * [Urls
](#urls) 
      * [Emails
](#emails) 
      * [Locations
](#locations) 
      * [Names(?) Challenge
](#names-challenge) 



   * [Advanced uses in Regular Expressions
](#advanced-uses-in-regular-expressions
)   
      * [Search and replace
](#search-and-replace) 

   * [Regular Expressions in programming languages
](#regular-expressions-in-programming-languages
)   

      * [Using REGEX to decompose GET queries
](#using-REGEX-to-decompose-GET-queries) 
      * [Project Explanation
](#project-explanation) 
      * [Perl
](#perl) 
      * [Php
](#php) 
      * [Using PHP in practice
](#using-PHP-in-practice) 
      * [Python
](#python) 
      * [Java
](#java) 
      * [Java Applied
](#java-applied) 
      * [JavaScript
](#javascript) 
      * [`grep` and `find` from console
](#grep-and-find-from-console) 



Introduction to Regular Expressions
============

Regular expressions express a language defined by a regular grammar that can be solved with a nondeterministic finite automaton (NFA), where the match is represented by the states.

A regular grammar is the simplest grammar expressed by the Chomsky Hierarchy.

![Alt text](/img1.png?raw=true "img1")

In a nutshell, a regular language is expressed visually so it can express an NFA, and here is a very simple example of an NFA:

![Alt text](/img2.png?raw=true "img2")

And the Regular Expression language is a textual representation of such an automaton. That last example is expressed by the following regex:

```bash
➥ ^[01]*1$
```

Which matches any string starting with 0 or 1 , repeating 0 or more times, ending with 1 . In other words, it's a regular expression to match odd numbers from their binary representation.

Everything you will learn about regular expressions
-----------



What are regular expressions?
-----------

Regular expressions are character patterns that allow you to select or discard data in a text file such as csv, or in a line or an input, depending on whether or not they match this pattern.



Applications of regular expressions
-----------

Regular expressions allow us to build patterns, which we can apply to files, and search for relevant information in them, a practical case (among many others) would be, extract from an SD card, the photographs taken on a certain date, or the precise and concise search of files in computer forensics.


Introduction to the regular expression language
-----------

/d -> Digit
/w -> Letter

* Shape
* give repetition

The language: characters, operators, and constructions
============

The character .
-----------

The character (.)

Text file. Series of character strings. A succession of lines.

Character string. A character followed by another character, followed by another character.

Character. Graphic representation in bits of some code, in most cases ASCII. It is the minimum unit that can be abstracted from a character string.

Predefined and built classes
-----------

| Regex	 | What does this? | Description | Reverse |
| --- | --- | --- | --- |
| . | Character | Any character, select each of the characters |  |
| /d | Digit| Digits: (lowercase d) Find all digits (number) from 0 to 9, it is | \D | 
| /w | Word| All word characters, Finds all the characters that are part of a word, both letters (lower or upper case) and numbers, it is equivalent to putting [a-zA-Z0-9_].| \W | 
| /s | Space| WhiteSpaces, Finds all spaces (line breaks and tabs are also spaces). | \S | 
| [0-9] | Specific Digit| Find all the digits from 0 to 9. |  | 
| [0-9a-zA-Z] | Specific Word Character | Find all characters that are from 0-9 or that are uppercase or lowercase letters (\w) |  | 
| [a-zA-Z]	 | | It will find us only the letters, both uppercase and lowercase. | | 
| \	 | Diagonal invertida| Escapes characters, allows a special character to be displayed
 |  | 

The delimiters: +, *, ?
-----------

 * '*' → Whether or not there is [Select all, operator greedy]


 Example: 
 ```
 \d*[a-tA-T]
```

It reads: Select the character that is in the range from __a__ to __t__, (both lowercase and uppercase) and ALL the numbers that precede it, WHETHER THEY EXIST OR NOT.

So, from the following example you will select


~~12345T~~exto

12345 ~~Te~~x~~to~~


 * '+' →There is one or more [There must be]

Example: 
 ```
\d+[a-tA-T]
```


It reads: Select the sequences of characters that contain AT LEAST ONE digit, followed by a character that is in the range from __a__ to __t__, (Both lowercase and uppercase).

So from the following example you will select

_12345T_ exto

12345 _Te_ x _to_



 * '?' →There is zero or one (There can be only one)

Example: 
 ```
\d?[a-tA-T]
```

It reads: Select the sequences of characters THAT CONTAIN OR NOT, A SINGLE digit, followed by a character that is in the range from __a__ to __t__, (Both lowercase and uppercase).

So from the following example you will select


Counters {1,4}
-----------

The case of (?) as a delimiter
-----------

Not (^), its use and its dangers
-----------

Challenge: Filtering out letters in phone numbers using negations
-----------


Beginning (^) and end of line ($)
-----------

Practical use of Regular Expressions
============


Logs
-----------
Phone
-----------
Urls
-----------
Emails
-----------
Locations
-----------
Names(?) Challenge
-----------



Advanced uses in Regular Expressions
============

Search and replace
-----------



Regular Expressions in programming languages
============

Using REGEX to decompose GET queries
-----------

Project Explanation
-----------


Perl
-----------

Php
-----------

Using PHP in practice
-----------

Python
-----------

Java
-----------

Java Applied
-----------

JavaScript
-----------

grep and find from console
-----------