# Title Regex Tutorial

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This is the regex we will be looking at as a example and it is one matching to a email address

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
The caret ^ and dollar $ characters have special meaning in a regex. They are called “anchors”. The caret ^ matches at the beginning of the text, and the dollar $ – at the end.

### Quantifiers
 A Quantifier specifies how many instances of the previous element (which can be a character, a group, or a character class) must be present in the input string for a match to occur. They also determine whether a regex will attempt a Greedy match or a Lazy match.In the example the numbers 2 and 6 are specifying there should be a minimum of 2 characters and maximum of 6. In addition, the + symbol is used as a quanitfier.

### OR Operator
There is no OR operator in this regex but if so it would be represented with ||

### Character Classes
Character classes are defined charcater sets within regex. In the example regex, \d is used which represents a match of digits between 0 and 9.

### Flags
Flags define parameters when searching. This regex example does not have any flags. 

### Grouping and Capturing
Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses.
There are 3 in our example ([a-z0-9_.-]+) user's email,  ([\da-z.-]+) email provider,  ([a-z.]{2,6}) domain name

### Bracket Expressions
Brackets expressions indicate parameters to meet, either letters or numbers, and will define the parameters. Our expression has parameters of anything a to z or 0 to 9.

### Greedy and Lazy Match
A greedy quantifier is shown as + and {}. A lazy quantifier is shown as +? and {}?. Our expression only has greedy quantifiers which will search for all matches whereas lazy quantifiers will only search for the shortest match.

### Boundaries
The word boundary \b matches positions where one side is a word character. There is none in our example.

### Back-references
Back-references research previously matched groups. They use a backslash and a single digit and are not in our example.

### Look-ahead and Look-behind
These functions define parameters where the match should include a component that comes before or behind another.This is not used in our example.

## Author

explained by kelly b 
github- https://github.com/