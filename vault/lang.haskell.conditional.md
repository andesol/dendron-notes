---
id: c03uvsi96v74u6tzpxbatm5
title: Conditional
desc: ""
updated: 1647537418276
created: 1647536298866
---

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
