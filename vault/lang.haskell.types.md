---
id: p2t6nyat9y9t6xeapp0wawq
title: Types
desc: ""
updated: 1647535012220
created: 1647532191271
---

It's a good practice in Haskell to write explicitly the types and not to rely exclusively on inference.

## Basic Types

- Bool
- Char
- String
- Int
- Float

## List Types

List is a sequence of values of the same type

```hs
[False, True, False] :: [Bool]
['a', ['b', 'c']] :: [Char]
```

## Tuples

A tuple is a sequence of values of different **types**

```hs
(False, True) :: (Bool, Bool)
(False, 'a', True) :: (Bool, Char, Bool)
```

The type of a tuple encodes it's size (a diferència de una _list_). Types unrestricted.

```hs
('a', (False, 'b')) :: (Char, (Bool, Char))
(True, ['a', 'b']) :: (Bool, [Char])
```

## Function Types

A function is a mapping between two types

```
not :: Bool -> Bool
```

- Polymorphic functions:

a ~= any (or b or c), p. e:

```
length :: [a] -> Int
```

- Overloaded functions: a polymorphic function is overloaded if its type contain one or more class constrainsts, e.g.

```
(+) :: Num a => a -> a -> a
```

(a has to be a numberic type)

- Num: Numeric types (+)
- Eq: equality types (==)
- Ord: ordered types (<)
