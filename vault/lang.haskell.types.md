---
id: p2t6nyat9y9t6xeapp0wawq
title: Types
desc: ""
updated: 1647692197714
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

The type of a tuple encodes it's size (unlike lists). Types unrestricted.

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

## Type declarations

```hs
type Pos = (Int, Int)

origin :: Pos
origin = (0,0)

left :: Pos -> Pos
left (x,y) = (x-1,y)
```

We can use params:

```hs
type Pair a = (a, a)


mult:: Pair Int -> Int
mult (m,n) = m*n
```
