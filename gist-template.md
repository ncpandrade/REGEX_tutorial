# Title REGEX Tutorial

A REGEX is a regular expression that searches for matching values/patterns within a string. The following REGEX is an example that looks for the string to match the general makeup of an email address. 


## Summary

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This tutorial will explain the most common REGEX vocabulary using the above email matching REGEX as an example. This particular REGEX can be used to validate that a user inputs a valid email address by searching the string for an unspecified number of characters, then the `@` symbol, followed by a domain.

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

### Anchors

The example REGEX inlcudes the following anchors:
`^` which marks the beginning of the REGEX
`$` which marks the end of the REGEX

### Quantifiers

The example REGEX inlcudes the following quantifiers:
`+` which is used to match one or more of the preceding token
`{2,6}` which matches the specified quantity of the previous token, in this case between 2 and 6 characters.  Alternatives would be {2}, which looks for 2 digits exactly, or {2,} which looks for 2 or more characters.

### OR Operator

### Character Classes

The example REGEX inlcudes the following quaracter classes:
`[a-z0-9_\.-]` which matches any charater in the set to the following parameters 
    -range from "a to "z" and is case sensitive.
    -range from "0" to "9"
    -matches a "_" character
    -`\.` matches a "." character (`\` required b/c a "." has a specific purpose in REGEX)  
    -matches a "-" character
`[\da-z\.-]` which matches any charater in the set to the following parameters
    -`\d` matches any digit
    -`a-z` matches a range from a-z
    -`\.` matches "." character
    -`-` matches "-" character

### Flags

The example REGEX inlcudes the following flags:
`g` which stands for global search

### Grouping and Capturing

The example REGEX inlcudes the following capturing groups:
`([a-z0-9_\.-]+)` which is the match criteria for the substring that precedes the "@" character in an email address
`([\da-z\.-]+)` which is the math criteria for the substring that follows the "@" character and precedes the "." character and in a typical email address describes the name of the mail server
`([a-z\.]{2,6})` which follows the "." character and in a typical email describes the domain.

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
