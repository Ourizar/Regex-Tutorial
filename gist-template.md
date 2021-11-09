# Matching an Email Regex

This tutorial will guide you to better understand, read, and write a regex.

## Summary

The regex that will be broken down in this document is used for matching an email. Please see the regex below:
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

 This regex has several components to it and they are:
 Anchors, Bracket Expressions, Quantifiers, Character Escapes, anc Character Classes. The table of contents below outlines these categories. Use the table of contents to see which component is used in the regex above and how it works.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)  
- [Character Escapes](#character-escapes)

## Regex Components
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
### Anchors
The characters ^ and $ are considered to be anchors. These anchors can be seen at the beginning and the end of our regex expression. The ^ anchor signifies a string that begins with the characters that follow it. So in our example regex we see that the string needs to have https:// and we also see specific characters in the within brackets which are lower case. This means that the letters of this URL will be all lowercase. The URL also accepts the hyphen - symbol within the URL.
### Quantifiers
The quantifiers used in this expression are ?, +, {}, and *.
There is a ? in front of the https, :// signifying that this will occur zero to 1 time. There is also a + symbol which is matching the pattern of 'https://lettersgohere ' one or more times before the '.' There are also curly braces where 2 and 6 are displayed. This will match the pattern for a minimum of 2 characters and a maximum of 6 times.
### Bracket Expressions
Our regex also has [], which is bracket notation. Bracket notation is case sensitive and in this expression we see [\da-z\.-] and another that contains a-z\.    This means that the url will only be able to all lower cases and a hyphen and period.

### Character Classes
You may notice that the regex contains a \d and a \w. \d—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

\w—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_) This class is equivalent to the bracket expression [A-Za-z0-9_].

### Character Escapes
The \ isolates certain characters that we don't want calculated in the regex. this can be seen in the https:// portion of our regex. 
## Author

The author, Oscar Urizar, is currently a student in the GA Tech Coding Bootcamp for Full Stack Web Development. The link to their GitHub account can be found below:
https://github.com/Ourizar