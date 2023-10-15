# Regex Tutorial: Matching an Hex Value

This README will be explaining the Hex Value regex and bellow will be diviing into more specific parts.

## Summary

This README is going to example what a Regular expression is and what the things that make it up mean. It will be breaking down the hex Value: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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

    - '^' and '$' and are both considered to be anchors.
    - The ^ is indicates the start of a string and the $ indicates the end of one.
    - In the hex value you can see the anchors at the beginning and end of the string anchoring down what pattern they should be looking for.

### Quantifiers

- Quantifiers set the limits of the string and are indicated by {}, ? , \*.
- ([a-f0-9]{6}|[a-f0-9]{3}) The quantifiers are saying with the {} it will have a minimum of 6 then 3 characters.

### OR Operator

- OR Operators are are indicated by the '|' symbol.
- ([a-f0-9]{6}|[a-f0-9]{3}) This is indicating here to look for the characters to be exactly 6 to 3 characters long.

### Character Classes

- Character classes defines a set of characters, any on e of which can occur in an inpout strin to fulfill match.
- Common one are '.','\d','\w', and '\s'.

### Flags

- Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex.

### Grouping and Capturing

- Grouping constructs is a way to check mulitple parts of a string to determine that different sections fulfill differetn requirements. The primary way to group a section is to use ().
- ([a-f0-9]{6}|[a-f0-9]{3}) You can see it there on our regex where the grouping is happening.

### Bracket Expressions

- Bracket expressions can make a matching list express or a non-matching expressoin list. It can consists of one or more expressions. To do bracket expressions you use these "[]".
- [a-f0-9]{6}|[a-f0-9] you see bracket expressions being used here in our value. It has character/range that the regular expressoin is looking for.

### Greedy and Lazy Match

- The Greedy match is a search that will try to find longest possible string, whereas a lazy match is a search for the smallest possible string.

### Boundaries

- Boundaries are similiar to anchors and uses the expression \b word boundary to indicate that a pattern is bouonded by a non-word character.

### Back-references

- Are regular expression commands which refer to a previous part of the matched regular expression. They are specified wiht the backlash and a single digit \1. The par tof the regular express they reger to is called a subexpression.

### Look-ahead and Look-behind

- look-ahead "looks ahead', and attempts to match teh subsequent input with the given pattern, but it does not consume any of the input.
- Look-behind 'looks behind', and attemts to match the previous input with the given pattern, but it does not consume any of the input if the match is successful, the current position in the input stays the same.

  - look aheads and look behind are indicated by ? and they are also indicated by saying negative or positive.

Ex: (?<=Y) = positive look behind
Ex: (?<=!Y) = negative look behind

## Author

- My name is Paul Cervantes and I am a student in the Full-Stack-Developer course at the UCLA extensions class.
- If any questions email me at paulcervantes2244@gmail.com
