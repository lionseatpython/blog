---
title: "FIXING THE BUILTIN `round` METHOD"
date: 2023-05-28
---
## The default `round()` behavior
The builtin `round()` method in Python can yeild some unexpected results that may catch a new user off-guard.

The syntax is `round(number, ndigits)`. Where:

number: the number we want to round

ndigits: is the number of decimal places we're looking to round `number` to.

For an example like rounding `3.668` to two decimal places, we say:
```python

round(3.668, 2)
```
>>3.67

When we run this, we get an output of `3.67`. No surprise!

However, for a number with a half-way point decimal (decimal 5), for instance `3.445`, rounding the number to two decimal places may yield surprising results.

```python

round(3.445, 2)
```
`>>3.44

### Explanation
