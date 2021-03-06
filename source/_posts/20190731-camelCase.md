---
title: 'CamelCase'
thumbnail: '/images/hackerrank.jpeg'
categories:
  - Algorithm
  - HackerRank
  - Problem Solving
tags:
  - Algorithm
  - HackerRank
  - Problem Solving
  - JavaScript
  - ES6
date: 2019-07-31 12:55:30
---

Alice wrote a sequence of words in CamelCase as a string of letters, , having the following properties:

- It is a concatenation of one or more words consisting of English letters.
- All letters in the first word are lowercase.
- For each of the subsequent words, the first letter is uppercase and rest of the letters are lowercase.

Given **s**, print the number of words in **s** on a new line.

For example, **s = oneTwoThree**. There are **3** words in the string.

<!-- more -->

## Function Description

Complete the camelcase function in the editor below. It must return the integer number of words in the input string.

camelcase has the following parameter(s):

- s: the string to analyze

## Input Format

A single line containing string **s**.

## Constraints 

- 1 <= |s| <= 10<sup>5</sup> 

## Output Format

Print the number of words in string **s**.

## Sample Input 

```
saveChangesInTheEditor
```

## Sample Output 

```
5
```

## Explanation 

String **s** contains five words:

1. save
2. Changes
3. In
4. The
5. Editor

Thus, we print **5** on a new line.

---

## Solution

```javascript
// Complete the camelcase function below.
function camelcase(s) {
    return (s || '').replace(/[a-z]/g, '').length + 1;
}
```
