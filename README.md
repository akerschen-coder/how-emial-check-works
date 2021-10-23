# how-email-check-works
This tutorial will explain how to use regex to match emails

## Summary

When building a website, developers often need user to sign in/sign up. With that being said, there needs to be a way to validate the emails given when trying to sign in. That is why we validate the email using the regex expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. Below I will describe how and why it is used. 

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
The components of the regex are in total `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
### Anchors
The anchors `^` and `$` make the regular expression find its match at the start and end of the text. `^` meaning the beginning of the string and `$` meaning the ending of the string.  
### Quantifiers
`+` and `*`  are quantifiers. The plus sign makes it run through the email one or more times, whereas the asterisk runs through it zero or more times (but only if it's inlcuded). In regex expressions, the quantifier are usually character classes or a group. 

### Grouping Constructs
Grouping in this expression cones 3 different ways. `([a-z0-9_\.-]+)` makes sure it matches the user email name. The second groupign is `([\da-z\.-]+)`  will match the email service and make sure it's an actual domain. Third group is `([a-z\.]{2,6})` to make sure it has a .com.

### Bracket Expressions
Bracket expressions would be the `[a-z0-9_\.-]`, `[\da-z\.-]`, and `[a-z\.]`. These are somewhat like conditionals- they are a group that makes sure that the numbers are 0-9 and letters are a-z. Very similar to the grouping constructs and charcter classes 
### Character Classes
The charcter classes are considered to be whats between the brackets and how they are used. Such as the `\d` can make it do that it will read it in a singular way- reading it as `4` and not  `44` if charcters are next to each other. 
### The OR Operator
The OR operator can be used with the email validation- depending on what the primary key to sign in is. It could be checking for multiple things- check the username OR the password OR the email with 2 of them matching. 
### Flags

### Character Escapes
I believe this is talking about 

## Author

Check out my github repos at https://github.com/akerschen-coder 