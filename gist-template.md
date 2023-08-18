# Email Expressions

Regex: ^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$

## Summary

In this github gist, we will be learning about expressions for matching email addresses. It will explain all of the components and hopefully a few insights on the functionality.

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

### Anchors

The expression uses the ^ and $ anchors to match the start and end of the email string, ensuring that the entire string adheres to the email pattern.

### Quantifiers

The quantifiers + and {2,6} are used in various places:

([a-z0-9_\.-]+) matches one or more occurrences of lowercase letters, digits, underscores, periods, and hyphens for the username.
([\da-z\.-]+) matches one or more occurrences of lowercase letters, digits, periods, and hyphens for the domain name.
([a-z\.]{2,6}) matches a sequence of 2 to 6 lowercase letters or periods for the top-level domain (TLD).

### Grouping Constructs

The regex uses parentheses to group different parts of the email address for specific matching, such as the username, domain name, and TLD.

### Bracket Expressions

Bracket expressions like [a-z0-9_\.-] and [\da-z\.-] are used to define character ranges for valid characters in the email address. These ensure that only permitted characters are matched.

### Character Classes

The character class \d is used to match digits in the domain name, contributing to the matching of valid email addresses.

### The OR Operator

The regex uses the | (OR) operator to allow for two possible email formats: one with a username and domain name of six characters each, and another with three-character segments.

### Flags

No flags are used in this regex pattern.

### Character Escapes

No character escapes are used in this regex pattern.

## Author

This information about this email expressions was authored by <a href= 'https://github.com/Kpeterson23'>
