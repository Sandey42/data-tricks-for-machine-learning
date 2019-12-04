# data-tricks-for-machine-learning

## Shorthand,useful code for data cleaning, pre-processing and handy ML tricks.


### 1. Removing digits from a sentence in one-line.

```python
remove_digits = str.maketrans('', '', string.digits)
sentence = sentence.translate(remove_digits)
```
