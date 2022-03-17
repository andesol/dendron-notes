---
id: ahpgleevox6se6ga67pz9jm
title: Curry
desc: ""
updated: 1647534280514
created: 1647533946299
---

Curried functions are more flexible, because you can partially apply them.

Currying conventions

- The arrow associates to the right.

```hs
Int -> Int -> Int
```

Means:

```hs
Int -> (Int -> Int)
```
