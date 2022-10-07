# Matching an Email

In this tutorial I will explain the use of Regular expressions to match emails. This is particularly useful for validating user inputs in various types of forms.

## Summary

Regular expressions or RegEx are sequences of metacharacters, denoting a pattern. These patterns can be of various kindssuch as a mix of letters with digits, special characters and even different language characters. In this tutorial we will use the following expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ to match emails.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components
Regular expressions will almost always start and end with forward slashes / so everything in betweens those slashes will be your regular expression.

### Anchors
Anchors have special meaning in regular expressions. They do not match any character but instead they match a position before or after characters.
The caret `^` anchor matches the beginning of a string, a line or multiple lines if applicable.
The dollar `$` anchor matches the end of a string, a line or multiple lines if applicable.

### Quantifiers
Quantifiers match a number of instances of a character, group, or character class in a string.
For matching emails we will use the + quantifier that will match one or more of the previous regex item. Let's take the first part of our regular expression as an example `([a-z0-9_\.-]+)`. The + is telling the expression to match any instances of letters, numbers,`-`, `_` or `.`. 

### Character Classes
A character class is a special notation that matches any symbol from a certain set. In this regular expression the `\d` match a single digit or a character from 0 to 9

### Grouping and Capturing
Capturing groups are useful for creating blocks of patterns They are created by placing the characters to be grouped inside a set of parentheses so you can apply repetitions or other modifiers to them as a whole. 

The first capturing group in this expression is `([a-z0-9_\.-]+)` that matches the user email name. The second capturing group is `([\da-z\.-]+)` that will match the email service. The last capturing group is `([a-z\.]{2,6})` to match the .com.

### Bracket Expressions
Bracket expressions are particulary useful to do large ranges of letters and numbers and to do specific checks. For email validation we will use `[a-z0-9_\.-]` that will match any letter a-z in lowercase as it is case senstive. It also matches any digit characters between 0-9 and matches the characters ,`-`, `_` and `.`. 

### Greedy and Lazy Match


## Author
You can check out my projects at [https://github.com/appolinefr](https://github.com/appolinefr)