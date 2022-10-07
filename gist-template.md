# Matching an Email

In this tutorial I will explain the use of Regular expressions to match emails. This is particularly useful for validating user inputs in various types of forms.

## Summary

Regular expressions or RegEx are sequences of metacharacters, denoting a pattern. These patterns can be of various kindssuch as a mix of letters with digits, special characters and even different language characters. In this tutorial we will use the following expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ to match emails.

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
Regular expressions will almost always start and end with forward slashes / so everything in betweens those slashes will be your regular expression.

### Anchors
Anchors have special meaning in regular expressions. They do not match any character but instead they match a position before or after characters.
The caret ^ anchor matches the beginning of the text.
The dollar $ anchor matches the end of the text.

### Quantifiers
Quantifiers match a number of instances of a character, group, or character class in a string.
For matching emails we will use the + quantifier that will match one or more of the previous regex item. Let's take the first part of our regular expression as an example ([a-z0-9_\.-]+). The + is telling the expression to match any instances of letters, numbers, "-', "_" or ".". 

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)