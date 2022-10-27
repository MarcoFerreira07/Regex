# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Found function on "https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions" added /d to front
function escapeRegExp(string) {
  return string.replace(/[/d/d/d.*+?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string

the point of the function above is to return and replace the string with 3 meta numbers followed by 18 literal special characters

Which means you can replace strings or even numbers. But this is also functional on searches when you are struggling to locate a difficult string that may contain numbers you can do a regex meta search using meta characters.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
the easiest regex compenent to understand is the search pattern through text using the "basic elements as linked below. 
for example \d is searching for a digit using the same principal of the example given in the link. .ook would match some of the following nook, look, book, cook, & took.

https://analytics.webtrends.help/docs/regular-expression-components

### Anchors
here are the anchors I found using the link above you can match and read indepth examples in link 
\followed by a single character
($)placed parentheses due to symbol breaking code. 
^
[]
|
a regular expression in parenthesis ()
a single character
*
+
?


### Quantifiers
https://learn.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions
this specifies how many instances of a character,group or character class mus be present. 
*	*?	Matches zero or more times.
+	+?	Matches one or more times.
?	??	Matches zero or one time.
{ n }	{ n }?	Matches exactly n times.
{ n ,}	{ n ,}?	Matches at least n times.
{ n , m }	{ n , m }?	Matches from n to m times.

### Grouping Constructs

https://www.youtube.com/watch?v=NrzFle7RD0g&ab_channel=Academind

Usingn paraentheses gives you a capturing group if the regex is placed inside of a parentheses it is stored. You can continue the code past the parentheses and it will search further
example
/(ab)
abababa  this would hit the construct above 3 times 

/({a-z}+)@/1
ab@abab the match here would only be at the first 2 places ab this is searching for an exact match and not a pattern. 
### Bracket Expressions

https://www.ibm.com/docs/it/netcoolomnibus/7.4?topic=library-bracket-expressions

This is very easy to understand you are specifically setting limitations on what you want to search for using [] and any specific set of characters or numbers example below is clear

Expression
Description
Examples
[abcd]	Matches any character in the square brackets.	[nN][oO] matches no, nO, No, and NO.
gr[ae]y matches both spellings of the word 'grey'; that is, gray and grey.

[a-d]	Matches any character in the range of characters separated by a hyphen (-).	[0-9] matches any decimal digit.
[ab3-5] matches a, b, 3, 4, and 5.

[0-9]{4} matches any four-digit string.

^[A-Za-z]+$ matches any string that contains only upper or lowercase characters.

\[[0-9 ]*\] matches an opening square bracket, followed by any digits or spaces, followed by a closed bracket.

[^abcd]
[^a-d]

Matches any character except those in the square brackets or in the range of characters separated by a hyphen (-).	[^0-9] matches any string that does not contain any numeric characters.
[.ab.]	Matches a multi-character collating element.	[.ch.] matches the multi-character collating sequence ch (if the current language supports that collating sequence).
[=a=]	Matches all collating elements with the same primary sort order as that element, including the element itself.	[=e=] matches e and all the variants of e in the current locale.

### Character Classes

character classes are the letters numbers which can be specified further with ^ or | in order to search for specific set of info examples
https://www.regular-expressions.info/charclass.html

[A-Za-z_]
[A-Za-z_0-9]

### The OR Operator

The | aka "the or operator" best example I can create is (8|1) searching for 8 or 1 
(1|5)searching for 1 or 5

### Flags
The way i can think of how I have used this in the past is setting a global search or global download. or a global code in css */

here are further examples of flags that can be used. as found in https://javascript.info/regexp-introduction flags section

i
With this flag the search is case-insensitive: no difference between A and a (see the example below).
g
With this flag the search looks for all matches, without it – only the first match is returned.
m
Multiline mode (covered in the chapter Multiline mode of anchors ^ $, flag "m").
s
Enables “dotall” mode, that allows a dot . to match newline character \n (covered in the chapter Character classes).
u
Enables full Unicode support. The flag enables correct processing of surrogate pairs. More about that in the chapter Unicode: flag "u" and class \p{...}.
y
“Sticky” mode: searching at the exact position in the text (covered in the chapter Sticky flag "y", searching at position)

### Character Escapes


Here is a list of character escapes and explanation 
https://www.jmp.com/support/help/zh/15.2/index.shtml#page/jmp/escaped-characters-in-regular-expressions.shtml

Escaped Characters

\\

single backslash

\A

start of a string

\b

word boundary. The zero-length string between \w and \W or \W and \w.

\B

not at a word boundary

\cX

ASCII control character

\d

single digit [0-9]

\D

single character that is NOT a digit [^0-9]

\E

stop processing escaped characters

\l

match a single lowercase letter [a-z]

\L

single character that is not lowercase [^a-z]

\Q

ignore escaped characters until \E is found

\r

carriage return

\s

single whitespace character

\S

single character that is NOT white space

\u

single uppercase character [A-Z]

\U

single character that is not uppercase [^A-Z]

\w

word character [a-zA-Z0-9_]

\W

single character that is NOT a word character [^a-zA-Z0-9_]

\x00-\xFF

hexadecimal character

\x{0000}-\x{FFFF}

Unicode code point

\Z

end of a string before the line break
## Author
Marco Ferreira 

A great googler and finder of information. Feel free to ask any questions and im sure i can get you the answer using google. 
If you teach a man to program without google, frustrate him for eternity (https://www.reddit.com/r/ProgrammerHumor/comments/nm8fma/teach_a_man_to_program_without_google_frustrate/)

Google is the greatest tool created for the average joe

Git hub info 
https://github.com/MarcoFerreira07
email info
marcoasf.com@gmail.com