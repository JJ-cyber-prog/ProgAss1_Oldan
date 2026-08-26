```python
# For Problem A: Word Rotation Problem
```


```python
def rotate_word(text):
    return text[1:] + text[0] if text else text


# Test cases
print(rotate_word("python"))  # "ythonp"
print(rotate_word("logic"))  # "ogicl"
print(rotate_word("Code"))  # "odeC"
print(rotate_word("A"))  # "A"

```

    ythonp
    ogicl
    odeC
    A



```python
# For Problem B: Username Builder Problem
```


```python
def make_username(first_name, last_name):
    clean_first = first_name.lower().replace(" ", "")
    clean_last = last_name.lower().replace(" ", "")
    return f"{clean_first}.{clean_last}"


# Test cases
print(make_username("Ada", "Lovelace"))  # "ada.lovelace"
print(make_username("Alan", "Turing"))  # "alan.turing"
print(make_username("Ana Maria", "De Leon"))  # "anamaria.deleon"

```

    ada.lovelace
    alan.turing
    anamaria.deleon



```python
# For Problem C: Bookend Swap Problem
```


```python
def swap_bookends(items):
    first, *middle, last = items
    return [last, *middle, first]


# Test cases
print(swap_bookends([1, 2, 3, 4, 5, 6]))  # [6, 2, 3, 4, 5, 1]
print(swap_bookends(["red", "green", "blue"]))  # ["blue", "green", "red"]
print(swap_bookends([8, 3]))  # [3, 8]
```

    [6, 2, 3, 4, 5, 1]
    ['blue', 'green', 'red']
    [3, 8]

