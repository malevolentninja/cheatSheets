# Regular Expressions 

A few notes.


## Character Classes

 -' . ' Any character except newline
 - ' \w \d \s ' word, digit, whitespace
 - ' \W \D \S ' not word, digit, whitespace
 - ' [abc] ' any of a, b, or c
 - ' [^abc] ' not a, b or c
 - ' [a-g] ' character between a & g

## Anchors
- ' ^abc$ ' start/end of the string 
- ' \b \B ' word, not-word boundary

## Escaped Characters

- ' \. \* \\ ' escaped special characters
- ' \t \n \r ' tab, linefeed, carriage return
- ' \u00A9 ' unicode escaped

## Groups & Lookaround

- ' (abc) ' capture group
- ' \1 ' backreference to group #1
- ' (?:abc) ' non-capturing group
- ' (?=abc) ' positive lookahead
- ' (?!abc) ' negative lookahead

## Quantifiers & Alternation 

- ' a* a+ a? ' 0 or more, 1 or more, 0 or 1
- ' a{5} a{2,} ' exactly five, two or more
- ' a{1,3} ' between one & three
- ' a+? a{2,}? ' match as few as possible
- ' ab|cd ' match ab or cd


## Example: Email Verification

A special text string for describing a search pattern. 
*.txt file looks like
```sh
^.*\.txt$
```

You can use the regular expression: 

```sh
\b[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,}\b
```
To search for an email address.


Changing \b with a ^  and the last \b with a $:

```sh
^[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,}$ 

```
Checks wether the user has entered a properly formatted email address. 

