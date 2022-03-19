---
id: rryaebrhges1ht5a1mdu3va
title: High order functions
desc: ""
updated: 1647691840772
created: 1647605343632
---

Useful?

- Domain specific languages can be defined as collections of higher-order functions.

- We can use albgebraic reasoning to understand programs.

## Map

```hs
map :: (a -> b) -> [a] -> [b]

> map (+1) [1,3, 4]
> [2,4,5]
```

## Filter

```hs
filter :: (a -> Bool) -> [a] -> [a]

> filter even [1,3,4]
> [4]
```

## Foldr

```hs
-- Pattern
f [] = v
f (x:xs) = x ⊕ f xs


--Example
sum [] = 0
sum (x:xs) = x + sum xs

product [] = 1
product (x:xs) = x * product xs

and [] = True
and (x:xs) = x && and xs


-- These operations can be defined using foldr (hof)
sum = foldr (+) 0
product = foldr (*) 1
...
```
