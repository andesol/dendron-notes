---
id: knqxow7iosykbnfq66fbun3
title: Code_examples
desc: ""
updated: 1647615481241
created: 1647604160948
---

Un exemple de recursion, list comprenhension, etc. és quick sort. Diu https://www.youtube.com/watch?v=WawJ8LArl54&list=PLF1Z-APd9zK7usPMx3LGMZEHrECUGodd3&index=8 que és _probablement_ l'implementació més simple.

```hs
qsort :: Ord a => [a] -> [a]
qsort []    = []
qsort(x:xs) =
    qsort smaller ++ [x] ++ qsort larger
    where
        smaller = [a | a <- xs, a <=x]
        larger  = [b | b <- xs, b > x]
```
