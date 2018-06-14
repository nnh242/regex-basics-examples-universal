Literal Matches: something that matches literally. cat finds cat. 

22 matches the first 22 of 222 so Regex searches from left to right.

Character Classes: try to match all character within square brackets []
You can also do a range of character [a-z] matches all characters from a to z. It is case sensitive so if you want all characters all cases then [a-zA-Z]. 

You can also do ranges with digits.
Example: [0-9]

Negate match: use the ^ inside and only inside the square bracket. [^a-z] negates all lower case character matches.
Backslash: escape
Putting character or symbol at the end of the character class also means literal.
Example: [a-z-] that is matching lower case characters and the literal dash - 

You can match any character even the ^ if it is at the end of the character class.
Example [@^] matches @ and ^ while [^@] negates matches of @

[\ -~] matches again any character that comes after as far as the string goes.

Alternations: | tries to match what is on the left of | and if that fails then it tries the stuff on the right of the |
Example: cat | dog | fish

Meta characters: - short cut for character classes.

The dot matches anything except for new line.

\. matches the literally dot .

\w is the short cut for [a-z0-9A-Z] 

Negation is \W which is equivalent to [^a-z0-9A-Z]

\d is [0-9]

Negation is \D equivalent to [^0-9].

\s matches any white spaces and \S is the negation of that.

