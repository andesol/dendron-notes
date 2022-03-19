
## Why is it useful?

Some functions are simpler to write in terms of other functions (e.g. factorial)

Properties of functions using recursion may be proved using a mathematical technique call **induction**.

```hs
length [] = 1
lenght [_:xs] = 1 + length xs
```

## How to think recursively

1. Write the type of the function
2. Enumerate the cases, e.g. empty list etc.
3. Generalise and simplify
