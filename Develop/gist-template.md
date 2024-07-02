# Understanding Regex: A Tutorial on Matching Email Addresses

In this tutorial we will explore how a regular expression (regex) can be used to match email addresses. We will break down each part of the regex to understand its functionality and how it contributes to the overall pattern.

## Summary

This tutorial will explain the regex used to match email addresses: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. We will go through each component of the regex and understand how it ensures that the input is a valid email address.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)

### Anchors

Anchors are used to match positions within a string. In our regex, `^` matches the start of the string and `$` matches the end of the string.

- `^` asserts the position at the start of the string.
- `$` asserts the position at the end of the string.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. In our regex, we use the `+` quantifier.

- `+` matches one or more of the preceding element.
  - Example: `[a-z0-9_\.-]+` matches one or more lowercase letters, digits, underscores, dots, or hyphens.

### OR Operator

The OR operator `|` allows for matching one pattern or another. In our regex, it is used within a grouping to match either 6 or 3 hexadecimal characters (not applicable in our chosen regex).

### Character Classes

Character classes match any one of a set of characters. In our regex, we have several character classes:

- `[a-z0-9_\.-]` matches any lowercase letter, digit, underscore, dot, or hyphen.
- `[\da-z\.-]` matches any digit, lowercase letter, dot, or hyphen.
- `[a-z\.]{2,6}` matches any lowercase letter or dot between 2 and 6 times.

### Grouping and Capturing

Grouping and capturing are used to group parts of a regex together and capture the matched content. In our regex, we use parentheses `()` for grouping and capturing.

- `([a-z0-9_\.-]+)` captures the username part of the email.
- `([\da-z\.-]+)` captures the domain name part of the email.
- `([a-z\.]{2,6})` captures the top-level domain part of the email.

## Author

This tutorial was created by ME Jaden D. You can find more of my work on [GitHub](https://github.com/DuleskyJ?tab=repositories).
