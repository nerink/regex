# Regex Tutorial- Matching an Email 

Regular expressions, also known as Regex, are used for defining filters to find certain patterns of characters. Regular expressions has a series of characters that define a pattern of text to be matched to create a more specialized filter, or general one- you choose. You can also find and replace a character or sequence of characters within a string. 

## Summary

This is the Regex code we will be anaylizing: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The anchors used to contain this regular expression are: ^ to start, and $ to finish.

### Quantifiers
+  is used to communicate there is another sequence to be matched as a greedy quantifier. 
{2,6} is also used as another greedy quantifer to specify that the input should be a minimum of 2 characrtors to a maximum of 6 characters.

### Character Classes
The charactor class \d is used which in classifies the use of any digit from 0 to 9.

### Grouping and Capturing
In this example, there are three groups that are being captured.
Group #1 is the username of the e-mail account [a-z0-9_\.-]. 
Group #2 captures the domain name or e-mail service being used [\da-z\.-]. 
Group #3 captures the domain extention (i.e .com or .net) [a-z\.]{2,6}.

### Bracket Expressions
The information in the three bracket expressions is contained between an opened and closed brackets[]. This indentifies which information is allowed to be matched.

Bracket Expression #1: [a-z0-9_\.-] - includes case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

Bracket Expression #2: [\da-z\.-] - includes all digits, case sensitive characters from a-z, periods and hyphens

Bracket Expression #3: [a-z\.] - includes case sensitive characters from a-z and periods.

### Greedy and Lazy Match
The example stated only used greedy quantifiers + and {}. It will allow the match to expand as long as it neess to go. If these quantifiers were lazy quantifiers, they would appear as +? or {}?, this will direct the system to make the shortest match.

## Author
My name is Nerin Kaur & this bootcamp has helped me a lot! 
Here is my github repository: