# How to Match an Email Using Regex

## Summary of Regex

Regex, short for Regular expressions, are strings of characters frequently used in search algorithms and code to find certain patterns of characters within a string, or to replace a character or sequence of characters within a string. In addition to finding and replacing characters, strings are also frequently used to validate input.

For example, the following regular expression can be used to verify that user input is a valid Email:  
/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/.

Regex, short for Regular expressions, are strings of characters that specify a search pattern in text. These patterns enable you to match, find, and manage text. For example, this regex matches e-mail addresses that comply with the requirements.

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Summary of Regex](#summary-of-regex)
- [Regex Components](#regex-components)
  - [Anchors](#anchors)
  - [Quantifiers](#quantifiers)
  - [OR Operator](#or-operator)
  - [Character Classes](#character-classes)
  - [Grouping and Capturing](#grouping-and-capturing)
  - [Bracket Expressions](#bracket-expressions)
  - [Greedy and Lazy Match](#greedy-and-lazy-match)
  - [Back-references](#back-references)
  - [Author](#author)

## Regex Components

### Anchors

Anchors are regex tokens that match no characters but state something about the string or the matching process. Anchors indicate where the current position in the string relates to a given position, such as the beginning or end of a string. This type of assertion is useful because it lets you match letters or digits only at the beginning or end of a string. Additionally, when you specify a location to search for patterns, it will not search anywhere else.

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/

In the regex code above, ^ anchor indicates the beginning of the text and $ anchor indicates the end of the text

### Quantifiers

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/
A quantifier indicates how many instances of a character, group, or character are required for a match to be found In the regex code above, + is a greedy quantifier that there is another sequence to be matched and [3,9] is a statement that there should be a minimum of 3 characters and a maximum of 9 characters in the input.

### OR Operator

The alternation is a simple OR, which is determined by a vertical line, so if you want to find four different things, Sedan, SUV, van and truck, you would put somthing like the following sedan|suv|van|truck.

### Character Classes

In regex, a character class matches only one character. However, you can use a hyphen to define a range of characters to be matched within square brackets. It is represented as the following set of characters enclosed within the square bracketes:  
 ([a-z0-9_.-]+)@([/da-z.-]+).([a-z.][2,6])$/. ([a-z0-9_.-]+)@([/da-z.-]+).([a-z.][2,6])$/.

### Grouping and Capturing

A regular expression can be grouped by placing it between parentheses () to apply quantifiers or to restrict alternation to that part of the regex;

/^([a-z0-9_\.-]+)@([\da-z\.-]+).([a-z\.]{2,6})$/

The regex code above consists of three groups. Group #1: [a-z0-9_\.-] serves as the email account name. The second group [da-z/.-] is used to capture domain names or email addresses. The domain extension is captured by group #3 [a-z/.].

### Bracket Expressions

Depending on the nonempty list expressions that follow the bracket expression (an expression enclosed in square brackets, "[]"), a bracket expression will match a specific set of single characters, and could match a specific set of multi-character collating elements.  
Defining sets of characters with square brackets, [], is straightforward. In this case, a range of characters or character classes is retrieved.

([a-z\.]{3,9})

The above example or expression, gets a range of lowercase letters, a through z, are followed by the a .

- [abc] It is used to find any character between the brackets.
- [^abc] It is used to find any character not between the brackets.
- [0-9] It is used to find any character between the brackets (any digit).
- [^0-9] It is used to find any character not between the brackets (any non-digit)
- (x|y) It is used to find any of the alternatives specified.

### Greedy and Lazy Match

"Greedy" is referring to matching the longest string possible, while "lazy" means matching the shortest string possible.

For example in "wallmart"

- 'Greydy' h.+l matches wall but
- 'Lazey' h.+?l matches wal

## Refference

- W3schools: [JavaScript RegExp Tutorial](https://www.w3schools.blog/regexp-javascript-tutorial)

## Author

![alt text](./assets/images/my_profile_pic.jpg)
[For more information about the author, please click here](https://ghashe.github.io/advanced-css-challenge-professional-portfolio/)  
[To view the author's github account, click here](https://github.com/ghashe)
