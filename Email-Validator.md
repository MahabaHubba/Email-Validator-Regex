# EmailValidation Regex
In a society where communication is key, emails play a vital role for many companies to relay important information.
Thus, an EmailValidation regex is essential for companies to utilise to onboard their new co-workers and supply them with a proper email to interact with the desired parties.

## Summary
The regex that will be explained below is: /^[\w\.-]+@[a-zA-Z\d\.-]+\.[a-zA-Z]{2,}$/
This regex is a email validator regex which matches the pattern of an email address, where the local part can consists of words, hyphen and dots followed by the '@' sign. Then there is a domain that consists of at least two letters.

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
- ^: denotes the start of the string
- [\w\.-]+: one or more occurences of any word character,dots or hyphens
- @: This matches the literal '@' symbol required in an email address
- [a-zA-Z\d\.-]+: This matches one or more occurences of any letter, digit, dot or hyphen which corresponds after the '@' sign.
- \.:This denotes a literal dot
- [a-zA-Z]{2,}: This denotes two or more occurences of any alphabetic letter, which corresponds to the domain of the email address.
- {$/} denotes the end of the string

### Anchors
There are two anchors for this this regex:
- ^: which signifies the start of the string
- ($): which signifies the end of the string

### Quantifiers
- +: is an example of a quantifier in the regex which signifies one or more occurences of teh preceding character or group. This is used as [\w\.-]+ in the regex which allows for one or more word characters, dots and hyphens.
- Similarly, {2,} is also a quantifier which has similare properties to `+`.

### Grouping Constructs
The grouping constructs are signified through the use of paratheses () which allow you to apply quantifiers and other operations to a group of characters.

### Bracket Expressions
- [\w\.-]: is a bracket expression that matches a single word (\w), a dot (\.) or a hyphen (-).
- [a-zA-Z\d\.-]: This bracket expressuib matches a single character that is either a letter (a-zA-Z), a digit (\d), a dot (.), or a hyphen (-). This part corresponds to the domain part of the email address after the @ symbol.
- [a-zA-Z]{2,}: The bracket expression matches two or more occurences of any alphabetical letter(a-z or A-Z), which corresopnds to the domain of the email address.

### Character Classes
The character classes are denoted in teh square brackets of the regex, where \w matches any character, equivalent to [a-zA-Z0-9_]. It matches letters, digits, and underscores. \d is a shorthand character class that matches any digit, equivalent to [0-9];

### The OR Operator
An OR operator is composed by '|' symbol, which allows you to specifiy alternatives for a pattern. However in this regex, there is no OR operator, but reaches similar effects through the various use of characters classes and ranfes, for e.g [\w.-]

### Flags
In many programming languages and environments, the use of flags in regex's are used to modify the regex's bahviour. Some common example of flags include, case sensitivity or Global(g), where it matches all occurences instead of stopping once the first match is found. In the EmailValidation regex, there is no specific flag present.

### Character Escapes
Character escapes in regular expressions are sequence of characters that hace a special meaning. Some examples are: (\n: represents a newline character, \t: represents a tab character). In the EmailValidation regex, \w, \. and \d are character escapes.

## Author
MahabaHubba is a up and coming coder, learning the arts of full stack development, keen to learn and ready to conquer any obstacle.
