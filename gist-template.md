# Regex for Matching a Hex Value

As a Web Deve student I am learning about regular expressions and how to use them to match patterns. I am creating this gist to document my learning process and to share my findings with others. I am creating this tutorial on how to match a hex value using regular expressions.

## Summary

I wil be explaining how to match a hex value using regular expressions by breaking down the regex into its components. Below is the code snippet of the regex.

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

This regular expression is looking for a string that starts with an optional "#" character, followed by either six or three characters in the range of "a" through "f" or "0" through "9", and then ends. This would match a hex color code, which is often used to specify colors in HTML and CSS.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

I will breakdown the regex into its components and explain what each component does.
Keep in mind that the order of the components is important.
`#?` - The question mark (`?`) is a metacharacter that indicates that the preceding character or group is optional. In this case, it matches an optional `#` character at the beginning of the string.

### Anchors

`^` (start of string), `$` (end of string)

### Quantifiers

`?` (zero or one), `{6}` (exactly six), `{3}` (exactly three)

### OR Operator

`|` (matches either the preceding expression or the expression following the operator)

### Character Classes
    
 `[a-f0-9]` (matches any character in the range of "a" through "f" or "0" through "9")

### Grouping and Capturing

`()` (grouping and capturing)

example:
`([a-f0-9]{6}|[a-f0-9]{3})` (groups and captures either six or three characters in the range of "a" through "f" or "0" through "9")

### Bracket Expressions
    
`[]` (matches any character in the brackets)

### Greedy and Lazy Match

Regex is greedy by default, meaning it will match as much as possible.
`{6}` (greedy match), `{3}` (greedy match)

## Author

This regex was created by Lian Perez (https://github.com/laps22)
