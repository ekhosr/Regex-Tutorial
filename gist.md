# Email Matching Regex Tutorial

Regular Expressions are a way to validate user's generated input and to search through a string text.

## Summary
```sh
Matching an Email: /^([a-z0-9_\.-]+)@([\da-z\-]+)\.([a-z]{2,6})$/
                     (   username  )@(  domain  ) .(extension )
                     ( eh-san_20.9 )@(  1e-mail ) .(    com   )
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
Anchors match a position before or after or between characters.
```sh
example: /^([a-z0-9_\.-]+)@([\da-z\-]+)\.([a-z]{2,6})$/
^ : only matches when the begining of string is lower case letters a-z, numbers 0-9, underscore, dot and hyphen.
$ : only matches when the end of string is lowercase letter a-z and between 2 to 6 characters.
```
### Quantifiers
```sh
'+' : in email example it means any characters of [a-z0-9_\.-] and more will be a match.
'{2,6}' : in email example it means any lower case a-z characters between 2 and 6 will be a match.
```

### Bracket Expressions
```sh
it means we want to match anything insde the []
example: [a-z0-9_\.-] means any character as long as the character is lower case letters a-z, numbers 0-9, underscore, dot and hyphen.
```

### Character Escapes
```sh
to escape default regex specail behavior we use character escape \
in email example [a-z0-9_\.-] the dot without backslash means any character, but with using backslash before dot we want to macth the dot character itself.
```

## Author
I am a student at Georgia Tech Bootcamp completing Full-Stack Web development program.
- [My Github Profile](https://github.com/ekhosr)