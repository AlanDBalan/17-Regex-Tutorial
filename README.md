17 - Regex tutorial

## Summary

Welcome to this comprehensive guide where we will dive deep into understanding the regular expression: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ , which is commonly used for validating email addresses. Throughout this tutorial, we will break down each component of the regular expression, explaining its purpose and functionality.

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

Anchors play a vital role in defining the position of a match within a string. In our regular expression, we use the ^ and $ symbols as anchors. The ^ anchor denotes the beginning of the string, while the $ anchor signifies the end. Together, they ensure that the entire string is validated from start to finish.

### Quantifiers

Quantifiers determine the number of times a preceding element should occur. In our regex, we employ the + quantifier. It applies to the character group [a-z0-9_\.-] and ensures that there is at least one or more occurrences of these characters. Similarly, the quantifier {2,6} specifies that the preceding character group [a-z\.] should occur between 2 to 6 times.

### OR Operator

The OR operator, represented by the | symbol, allows for multiple options to be matched. However, in our particular regular expression, we don't utilize the OR operator.

### Character Classes
 
 Character classes, enclosed in square brackets [], enable us to match any single character within the specified range. In our regex, [a-z0-9_\.-] matches any lowercase alphabetic character (a-z), digit (0-9), underscore (_), period (.), or hyphen (-). Similarly, [\da-z\.-] matches a digit (\d), lowercase alphabetic character (a-z), period (.), or hyphen (-). The character class [a-z\.] matches any lowercase alphabetic character or period.

### Flags

Flags modify the behavior of the regex matching. In our regex, we do not make use of any flags.

### Grouping and Capturing

Parentheses () are employed for grouping and capturing specific parts of the regex. In our regular expression, we define three groups:

([a-z0-9_\.-]+) captures the local part of the email address, such as the username.
([\da-z\.-]+) captures the domain name.
([a-z\.]{2,6}) captures the top-level domain (e.g., com, org).

### Bracket Expressions

Bracket expressions define a set of characters to be matched. In our regex, [a-z0-9_\.-] matches any lowercase alphabetic character, digit, underscore, period, or hyphen.

### Greedy and Lazy Match

Our provided regular expression does not involve any quantifiers that require consideration of greedy or lazy matching.

### Boundaries

Boundaries are used to match specific positions in the input string, such as word boundaries or non-word boundaries. However, in our regex, we do not explicitly employ boundaries.

### Back-references

Back-references enable us to reference previously captured groups within the regex. In our given regular expression, we do not utilize back-references.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions allow us to check for matches based on specific conditions ahead or behind the current position. In our provided regex, we do not incorporate look-ahead or look-behind assertions.

## Author

I hope this tutorial helped you learn something about regEx. Thanks for reading!
