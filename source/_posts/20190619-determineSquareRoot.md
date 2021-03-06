---
title: 정수 제곱근 판별
thumbnail: '/images/programmers.png'
categories:
  - Algorithm
  - Programmers
  - Level1
tags:
  - Algorithm
  - Programmers
  - Level1
  - JavaScript
  - ES6
date: 2019-06-19 00:50:47
---

## 문제 설명
임의의 정수 n에 대해, n이 어떤 정수 x의 제곱인지 아닌지 판단하려 합니다.<br/>
n이 정수 x의 제곱이라면 x+1의 제곱을 리턴하고, n이 정수 x의 제곱이 아니라면 -1을 리턴하는 함수를 완성하세요.

<!-- more -->

## 제한 사항
- n은 1이상, 50000000000000 이하인 정수입니다.

<br/>

## 입출력 예

| n | return |
| --- | --- |
| 121 | 144 |
| 3 | -1 |

<br/>

## 입출력 예 설명
입출력 예#1<br/>
121은 정수 11의 제곱이므로, (11+1)를 제곱한 144를 리턴합니다.<br/>

입출력 예#2<br/>
3은 정수의 제곱이 아니므로, -1을 리턴합니다.<br/>

<br/>

### Solution

---

```javascript
function solution(n) {
    return Number.isInteger(Math.sqrt(n)) ? (Math.sqrt(n) + 1) ** 2 : -1;
}
```