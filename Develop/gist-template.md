# Regex Tutorial
## User Story
AS A web development student
I WANT a tutorial explaining a specific regex
SO THAT I can understand the search pattern the regex defines
Acceptance Criteria
GIVEN a regex tutorial
WHEN I open the tutorial
THEN I see a descriptive title and introductory paragraph explaining the purpose of the tutorial, a summary describing the regex featured in the tutorial, a table of contents linking to different sections that break down each component of the regex and explain what it does, and a section about the author with a link to the author’s GitHub profile
WHEN I click on the links in the table of contents
THEN I am taken to the corresponding sections of the tutorial
WHEN I read through each section of the tutorial
THEN I find a detailed explanation of what a specific component of the regex does
WHEN I reach the end of the tutorial
THEN I find a section about the author and a link to the author’s GitHub profile

## Summary
The challenge this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. I choose to break down and explaing the following function...

    Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components
This regex's components include anchors, quantifiers, capture groups, and bracket expressions.

### Anchors
Anchors tell the expressions to start or end the search. In this specific example, the anchors are the caret, ^, which is positioned at the beginning of the string and the dollar symbol, $, which is positioned at the end. 

### Quantifiers
Quantifiers determine how many instances of a character, group, or character class can be present in the expression. This string includes the following quantifiers:[a-z0-9_\.-]+@
This means that the expression will look for 
1. Lowercase Letters a-z
2. Numbers 0-9
3. Period (.) 
4. At Symbol (@)
The backslash is used to interpret the period as an actual period while the plus sign is used finish the initial character search. {2,6} is used to look for a 2-6 characters to represent the section after the "@" sign.

### Character Classes
Character classes define specific sets of characters that can occur within strings that help the expression to match only one out of several characters. This string inculdes the following character classes:
1. \d matches a single character 0-9.

### Flags
Flags are used to determine the boundaries of an expression. In this example, both / at the beginning and end of the string are used as flags.

### Grouping and Capturing
Some regexs can contain grouping using parentheses, which treats everything within the parentheses as a single unit. this string includes the following groupings:
1. [a-z0-9_\.-]+) (represents username)
2. ([\da-z\.-]+) (represents domain)
3. ([a-z\.]{2,6}) (represents whatever comes after the period like .net or .org)

### Bracket Expressions
Bracket Expressions use [] to ensure that the input should match a specific set of characters. For example [a-z0-9_\.-] is encatpured by brackets and means that ther expression should look for letters a-z and 0-9. This string contains the following bracket expressions.
1. [a-z0-9_\.-]
2. [\da-z\.-]
3. [a-z\.]

### Greedy and Lazy Match
Tha qualifiers in this string are greedy as most expressions are greedy meaning that they attempt to match as much as possible where as lazy quantifiers use the minimal match requirements.

## Author
My name is Aireeal Blackmon and I am a current student of MSU's Coding Bootcamp. I hope you enjoyed this tutorial and breakdown of the regex used to match an email. 
I'd love to connect and if you would too, contact me: https://github.com/ablackmon1107