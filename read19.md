# Read 19
## Automation
Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.
In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

import re
The re library in Python provides several functions that make it a skill worth mastering. You will see some of them closely in this tutorial.


Basic Patterns: Ordinary Characters
You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.
Grouping in Regular Expressions
The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual.

Let's understand this concept with a simple example. Imagine you were validating email addresses and wanted to check the user name and host. This is when you would want to create separate groups within your matched text.

TIP: You can always access the named groups using numbers instead of the name. But as the number of groups increases, it gets harder to handle them using numbers alone. So, always make it a habit to use named groups instead.


Greedy vs. Non-Greedy Matching
When a special character matches as much of the search sequence (string) as possible, it is said to be a "Greedy Match". It is the normal behavior of a regular expression, but sometimes this behavior is not desired:

However, if you only wanted to match the first `<h1>` tag, you could have used the greedy qualifier `*?` that matches as little text as possible.

Adding ? after the qualifier makes it perform the match in a non-greedy or minimal fashion; That is, as few characters as possible will be matched. When you run <.*>, you will only get a match with `<h1>`.



Character(s)	What it does

.	A period. Matches any single character except the newline character.

^	A caret. Matches a pattern at the start of the string.

\A	Uppercase A. Matches only at the start of the string.

$	Dollar sign. Matches the end of the string.

\Z	Uppercase Z. Matches only at the end of the string.

[ ]	Matches the set of characters you specify within it.

\	∙ If the character following the backslash is a recognized escape character, then the special meaning of the term is taken.

∙ Else the backslash () is treated like any other character and passed through.

∙ It can be used in front of all the metacharacters to remove their special meaning.

\w	Lowercase w. Matches any single letter, digit, or underscore.


\W	Uppercase W. Matches any character not part of \w (lowercase w).

\s	Lowercase s. Matches a single whitespace character like: space, newline, tab, return.

\S	Uppercase S. Matches any character not part of \s (lowercase s).

\d	Lowercase d. Matches decimal digit 0-9.

\D	Uppercase D. Matches any character that is not a decimal digit.



\t	Lowercase t. Matches tab.

\n	Lowercase n. Matches newline.

\r	Lowercase r. Matches return.


\b	Lowercase b. Matches only the beginning or end of the word.

+	Checks if the preceding character appears one or more times.

*	Checks if the preceding character appears zero or more times.


?	∙ Checks if the preceding character appears exactly zero or one time.

∙ Specifies a non-greedy version of +, *

{ }	Checks for an explicit number of times.

( )	Creates a group when performing matches.

< >	Creates a named group when performing matches.



