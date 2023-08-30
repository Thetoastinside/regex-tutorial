# Regex Tutorial

A Regex or Regular Expression is a sequence of characters that defines a specific search pattern.

## Summary

This will be an overview of three different Regular Expressions.

## Table of Contents

- [Anchors](#anchors)
- [OR Operator](#or-operator)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Anchors are a different breed. They do not match any character at all. Instead, they match a position before, after, or between characters. They can be used to “anchor” the regex match at a certain position. The caret ^ matches the position before the first character in the string. Applying ^a to abc matches a. ^b does not match abc at all, because the b cannot be matched right after the start of the string, matched by ^. See below for the inside view of the regex engine. Similarly, $ matches right after the last character in the string. c$ matches c in abc, while a$ does not match at all.

### OR Operator

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
The "or" operator within a regular expression is defined using the | element. The or operator indicates that it could either of the components that we are separating with the |. For our hex value regular expression we have ([a-f0-9]{6}``|``[a-f0-9]{3}). Note the or operator separating these 2 components. This means that our hex value could either be 6 characters [a-f0-9]{6} or 3 characters [a-f0-9]{3}.


### Greedy and Lazy Match

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
A greedy match tries to match an element as many times as possible. Whereas, a lazy match tries to match an element as few times as possible. In our example we have ? which signifies lazy quantifier. This is referred to a lazy quantifier because it causes the regular expression engine to match as few occurances as possible. We can simply turn this lazy match into a greedy one by adding a ?.


## Author

Hello my name is Ryan Anderson, a full stack developer student.
Github [https://github.com/Thetoastinside]
