
## if ... then ... else

```hs
abs :: Int -> Int
abs n = if n >= 0 then n else -n
```

Alternatively:

## Guarded Equations

```hs
abs n | n >= 0    = n
      | otherwise = -n
```

## Pattern Matching

```hs
not :: Bool -> Bool
not False = True
not True = False
```
