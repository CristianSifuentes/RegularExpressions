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

Applications of regular expressions
-----------

Introduction to the regular expression language
-----------


The language: characters, operators, and constructions
============

The character .
-----------

Predefined and built classes
-----------

The delimiters: +, *, ?
-----------


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