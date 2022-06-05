# Title (Find a Url)


This will be an explaination of the regexs for an expression to find mathing url. the expression is" /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/".This expression should find text similar to https://www.joecar-llc.eu/The_Fun-Car/ but wont return https://www.*joe*.com

## Summary

A brief summary of the find a url expression above starts with its 4 groups. The Expression has a start step middle parts and an end. the start and the end sections of the code are optional because it has the ? symbol inside of the grouping. The start section returns http https text. The end returns a group of words the can also include - inside the word groups and ends with a /. The two middle sections return grouping of numbers and letters from a-z where in the first section you can return unlimited numbers letters from a to z and including ".". The second section does not accept numbers and had a charater max min of 2-6 charaters. 



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
start:  the start of this expression is indicarted by a ^ symbol. The first group ^(https?:\/\/)? it is looking for http with an optional s indicated by the ? follows by two \. this will return the string if it has https:\\ or http:\\. the string will also return without because that is also otional.
end: the end of this expression is indicated by the $ symbol. The last group ([\/\w \.-]*)*\/?$ is looking for any word. the grouping can also include a . and -. you can repeat that ad many times as needed indicated by the *. that grouping ends with a / and the ending is optional. indicated by the ?
roar: This is any text that is inside of the expression like the "." that seperates the second and third group or the text string at in the 4th group 

### Anchors
^(https?:\/\/)? the anchor is ^ which means the start 

([\/\w \.-]*)*\/?$/ the anchor is the $ which means end 
### Quantifiers
+ : this means that any charater one or more times 
? : this means that the chrater is optional
{2,6} : this means 2-6 charaters are needed 

### OR Operator
[\da-z\.-]

[a-z\.]

[\/\w \.-]

### Character Classes
\w  this is for wordd 

\d this is for a sigle digit

a-z this is for and lowercase letter a-z

\.- this adds . and -

### Flags
\da-z\ this flag includes any digit and any charater a-z lowercase

\/\ this flag includes a \

\/\w \ this flag includes a word 

### Grouping and Capturing
^(https?:\/\/)?  this is the grouping for http:\\ and   https:\\ and this is optional
([\da-z\.-]+) this is for a group of digits and letters that can be seperated by a . or -
\.([a-z\.]{2,6}) this is for a group with lower case letters a-z and has to 2-6 charaters long 
([\/\w \.-]*)*\/?$ this is for a group of words that starts with a \ and the whole words are seperated by a - or . 

### Bracket Expressions
[\da-z\.-]  includes digit, lowercase letter a-z and . and -

[a-z\.]  includes lowercase letter a-z

[\/\w \.-] includes word and - and .
### Greedy and Lazy Match
*  this means to repeat as manytimes as nessasary 
+ this means any charater one or more times 

### Boundaries
\/\w \ searches for whole words after a /
### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
