# Regex Tutorial

Regular expressions, also known as "regex" or "regexp", are a strong tool for matching patterns in idea. They are used in many programming languages and forms, including Python, JavaScript, Perl, and Computer software for basic operation command-line utilities. Regular verbalizations can be used to validate dossier, search for information, and act complex string manipulations. In this tutorial, we will learn the basics of consistent expressions and how to use ruling class in various applications.
## Summary

In this tutorial, we will be covering the basics of regular expressions in JavaScript, including the syntax and common uses. We will be covering the following topics:

Literal characters and special characters
Anchors and character classes
Repetition and groups
Using regular expressions in JavaScript with string methods such as match(),search() and replace()
Code snippet to match any phone number that starts with '+91' or '91':
```
let phoneNumber = "+919999999999";
let pattern = /^(91|\+91)/;
let match = phoneNumber.match(pattern);
if (match) {
    console.log("Valid phone number");
} else {
    console.log("Invalid phone number");
}
```
In this example we will be using regex to match phone numbers that starts with '+91' or '91' using the match() method from javascript's String class . We are using ^ to match the start of the string, (91|\+91) to match either '91' or '+91' and match() method to check if the pattern is present in the given phone number.
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
Regex components are the building blocks of regular expressions. They include literals, special characters, anchors, character classes, quantifiers, grouping constructs and flags.
 They are used to match and manipulate strings and are combined to form more complex patterns. Some examples include matching any digit using \d, matching the start of a string using ^, matching one or more occurrences of a pattern using + and making a regular expression case-insensitive using i flag.
### Anchors
Anchors are special characters that are used to match the position of a pattern within a string. They do not match any characters themselves, but instead assert the position of the pattern.
### Quantifiers
Quantifiers are special characters that specify the number of occurrences of a pattern in a regular expression. They include * (matches zero or more occurrences), + (matches one or more occurrences), ? (matches zero or one occurrence), {n} (matches exactly n occurrences), {n,} (matches n or more occurrences) and {n,m} (matches at least n and at most m occurrences) . They are used to specify the number of times a pattern should be repeated, and can be combined with other regex components such as character classes, anchors, and groups to create more powerful regular expressions.
### Grouping Constructs
Grouping constructs are special characters used in regular expressions to group patterns together and apply repetition or alternation to the group as a whole. They are used to group subpatterns together and to apply quantifiers to them. There are several types of grouping constructs, including capturing groups, non-capturing groups, positive lookahead, negative lookahead, positive lookbehind and negative lookbehind. The matched groups can be accessed later for further manipulation or extraction.
### Bracket Expressions
A bracket expression is a special syntax used in regular expressions to match any single character from a set of characters. It is enclosed in square brackets [] and can include individual characters, ranges of characters, and special character classes. For example, [abc] would match any of the characters 'a', 'b', or 'c', [a-z] would match any lowercase letter, and [\d] would match any digit. Bracket expressions can also be used in combination with other regular expression components, such as anchors, quantifiers, and groups to create more powerful patterns.
### Character Classes
A character class is a special syntax used in regular expressions to match any single character from a predefined set of characters. The most common character classes are \d to match any digit, \w to match any word character (letters, digits, and underscores), \s to match any whitespace character (spaces, tabs, and line breaks) and . to match any character except a new line. These classes allow you to match a wide range of characters with a single character. They can be used in combination with other regular expression components, such as anchors, quantifiers, and groups to create more powerful patterns.
### The OR Operator
The OR operator is a special syntax used in regular expressions to match any one of several patterns. It is denoted by the | symbol and separates the different patterns to match. For example, the regular expression cat|dog would match the strings "cat" or "dog".

The OR operator can also be used inside a group to match any one of several patterns. For example, the regular expression (cat|dog) would match the strings "cat" or "dog" and capture the matched word in a group.

The OR operator is also known as alternation and is used to create more complex and versatile regular expressions. It is a powerful feature that allows you to match multiple variations of a pattern in a single regular expression.
### Flags
Flags are special options that can be added to a regular expression to modify its behavior. They are identified by a leading (? and a trailing ). Some common flags include i for case-insensitivity, g for global matching, m for multiline matching, s for treating input as a single line, u for unicode matching and y for sticky search. These flags can be used to fine-tune the behavior of regular expressions and make them more powerful and versatile.
### Character Escapes
Character escapes are special characters used in regular expressions to match special characters that have a special meaning. They are identified by a backslash \ before the character. Some common examples include \d, \w, \s, \n, \r, and \t. They allow you to match special characters as literal characters, rather than their special meaning.
## Author

[Omar Yassine](https://github.com/OYASSINE1999)
