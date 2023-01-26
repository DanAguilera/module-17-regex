# module-17-regex

The following module is to dive into the Regex URL expression of `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

# Summary
To summarize as mentioned, the following will be used to decribe and dive into what this regex URL expression is `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`. This is an expression that is used to validate a URL. It uses a combination of special characters sets of those types of characters to check for certain patterns in the URL. For example, the http(s), domain name etc. 

# Table of Contents
- Anchors
- Quantifiers
- OR Operator
- Character Classes
- Flags
- Grouping and Capturing
- Bracket Expressions
- Greedy and Lazy Match
- Boundaries
- Back-references
- Look-ahead and Look-behind


# Regex Components

### Anchors
  The following expression contains two anchors, the '^' and the '$'. The '^' is considered the beginning or start of line. Its basically used to ensure  that the pattern match at the start of the string. The '$' is considered the end or end of line. This basically ensures that the pattern must match at the end of the string.

### Quantifiers
  The expression also contains two quantifiers; the '?' and the '*'. The '?' appears twice in the pattern, after the http and after the 's' It is used to show that the characters or set before the '?' is optional and can appear once or none. This basically means that the pattern will match the htttp in the URL. The '*' appears after ([\/\w \.-]*) set. It indicates that the characters before or group can appear at any amount of times, even zero. This means that the pattern will match any number of forward slashes, letter characters, dots and hyphens after the domain. 
  These work together with other things within the pattern to match a ton of valid URL's

### OR Operator
  This expression doesnt contain an OR Operator but the OR operator in regex is the '|' symbol, it basically allows to match different alts of a pattern.
Its used in combination with the '()' to group and match. 

### Character Classes
  The following are the character classes within the expression and what the do: 
  
  - [a-z] : these charcaters matches any lowercase letters between a-z. It shows up twice. 
  - [\da-z] : These characters matches any letters between a-z lower or uppercase or any digit 0-9.
  - [\/\w \.-] : These characters matches any of the characters '/', '\w', ' ', '.' and '-'.
  - [\d] : The character matches as mentioned above any digit between 0-9.

Character classes is a set of charcters enclosed in square brackets.

### Flags

  This expression doesnt contain any flags. But basically a flag is a character that modifes the behavior of the pattern. 

### Grouping and Capturing
   Grouping and capturing are used to group together parts of a patter and to capturn matched texts in groups. Usually its done with parentheses.

### Bracket Expressions
   Bracket expressions are defined using square brackets. The basically provide an accurate wat to define sets of characters. 

### Greedy and Lazy Match
  A greedy match matches as much text as possible, while a lazy match is one that matches as little text as possible. In this expression, the group ([\/\w \.-]*)* is greedy, so it will match all the characters that match the pattern [\/\w \.-] until the end of the string. The group ([\/\w \.-]*)? would be lazy and would match as few characters as possible as long as the pattern still matches.

### Boundaries
  Boundaries arw used to specift the position at which a pattern must match in the string. The '^' and the '$' would be the boundaries.
  
### Back-references
  Back-references are used to refer back to a previously matched group in the pattern. There are no backrefences used in this expression.

### Look-ahead and Look-behind
  Look ahead and look behind are used to assert whether a pattern is followed or preced by another pattern, WITHOUT including that pattern in the match. There are no look ahead and look behind in our expression. Lookahead is represented by the syntax (?=...) and lookbehind is represented by the syntax (?<=...).

# Author

Daniel Aguilera
