# Regex-tutorial
# Quick and Easy Intro to REGEX

Introductory paragraph:
Regular Expressions, commonly known as Regex, are powerful tools used for pattern matching and manipulation of text. In this guide, we will introduce you to the world of Regex in a simple and approachable way. If you have no prior knowledge of Regex, fear not! We will break down each component and explain them in plain language, providing examples along the way.


## Summary

In this guide, we will explain Regular Expressions and their various components. We'll cover everything from simple anchors and quantifiers to more complex concepts like grouping, back-references, and look-ahead/look-behind. To get started, let's understand what a regex looks like using a simple code snippet:

\d{3}-\d{2}-\d{4}

This regex is designed to match a pattern that resembles a Social Security Number (SSN) in the format: "123-45-6789". Now, let's dive into each component to understand how this regex works and explore many other examples!


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
Anchors are like signposts for regex, indicating specific positions within the text. Commonly used anchors are the caret ^ (matches the start of a line) and the dollar sign $ (matches the end of a line).

Examples:

^hello: Matches lines that start with "hello".

world$: Matches lines that end with "world".

^start$: Matches lines that only contain the word "start".


### Quantifiers
Anchors are like signposts for regex, indicating specific positions within the text. Commonly used anchors are the caret ^ (matches the start of a line) and the dollar sign $ (matches the end of a line).

Examples:

colou?r: Matches "color" or "colour" (the "u" is optional).

go*gle: Matches "gogle", "google", "gooogle", and so on (the "o" can repeat zero or more times).

go+gle: Matches "gogle", "google", "gooogle", and so on (the "o" can repeat one or more times).

### OR Operator
The OR operator | allows you to match either one expression or another. For example, cat|dog matches either "cat" or "dog."

Examples:

sun|moon: Matches either "sun" or "moon".

apple|orange|banana: Matches "apple", "orange", or "banana".

### Character Classes
Character classes allow you to match a single character from a group of characters. For instance, [aeiou] matches any vowel.

Examples:

[aeiou]: Matches any vowel (a, e, i, o, or u).

[0-9]: Matches any digit from 0 to 9.

[A-Za-z]: Matches any uppercase or lowercase letter.

### Flags
Flags modify the behavior of the regex pattern. The most common one is the case-insensitive flag i, which allows for case-insensitive matching.

Examples: 

/hello/i: Matches "hello", "Hello", "HELLO", and so on (case-insensitive).

/apple/m: Matches "apple" when it appears at the beginning of a line (multi-line mode).

### Grouping and Capturing
Parentheses () are used for grouping and capturing portions of the matched text. They also enable back-references.

Examples:

(ab)+: Matches "ab", "abab", "ababab", and so on.

(red|blue|green) apple: Matches "red apple", "blue apple", or "green apple".

(go)+ (team)+: Matches "go go team team", "go go go team team team", and so on.

### Bracket Expressions
Bracket expressions are used to define a custom character class. For example, [0-9] matches any digit.

Examples:

[abc]: Matches "a", "b", or "c".

[0-9A-Fa-f]: Matches any hexadecimal digit.

[^0-9]: Matches any character that is not a digit.

### Greedy and Lazy Match
Quantifiers are greedy by default, meaning they match as much text as possible. You can make them lazy by adding a ? after the quantifier, which makes it match as little as possible.

Examples: 

x+: Matches "x", "xx", "xxx", and so on (greedy).

x+?: Matches "x" (lazy).

### Boundaries
Boundaries allow you to match text at specific positions, such as word boundaries (\b) or non-word boundaries (\B).

Examples: 

\bword\b: Matches the word "word" as a whole word, not as part of another word.

\Bfoo\B: Matches "foo" only if it is not surrounded by word boundaries.

### Back-references
Back-references allow you to refer back to captured groups in the regex pattern. They are useful for finding repeated patterns.

Example:

(cat|dog) \1: Matches "cat cat" or "dog dog", but not "cat dog" or "dog cat" (back-references the first capture group).


### Look-ahead and Look-behind
Look-ahead ((?=...)) and look-behind ((?<=...)) are used for asserting specific conditions ahead or behind the current position without including them in the match.

Examples:

(?=good)morning: Matches "good morning" but not "morning" (positive look-ahead).

(?<!un)happy: Matches "happy" but not "unhappy" (negative look-behind).
## Author

Gabriel Cruz https://github.com/Gcruz10
Gist file https://gist.github.com/Gcruz10/1f9243d2fa86a55b47baf60993549223
