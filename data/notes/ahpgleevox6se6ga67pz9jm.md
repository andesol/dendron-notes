
Curried functions are more flexible, because the can be partially applied.

Currying conventions

- The arrow associates to the right.

```hs
Int -> Int -> Int
```

Means:

```hs
Int -> (Int -> Int)
```
