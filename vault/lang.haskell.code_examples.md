---
id: knqxow7iosykbnfq66fbun3
title: Code examples
desc: ""
updated: 1647703836123
created: 1647604160948
---

## Quick sort

```hs
qsort :: Ord a => [a] -> [a]
qsort []    = []
qsort(x:xs) =
    qsort smaller ++ [x] ++ qsort larger
    where
        smaller = [a | a <- xs, a <=x]
        larger  = [b | b <- xs, b > x]
```

Taken from [this video](https://www.youtube.com/watch?=WawJ8LArl54&list=PLF1Z-APd9zK7usPMx3LGMZEHrECUGodd3)
