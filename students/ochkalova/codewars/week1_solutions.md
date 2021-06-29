# 1. Human Readable Time.

```python
def format(integer, max_value):
    return str(min(integer, max_value)).zfill(2)

def make_readable(seconds):
    hours = format(seconds // (60 * 60), 99)
    minutes = format(seconds % (60 * 60) // 60, 59)
    seconds = format(seconds % 60, 59)
    return f"{hours}:{minutes}:{seconds}"
```
  
# 2. Isograms.

```python
def is_isogram(string):
    for i in set(string):
        if string.lower().count(i) > 1:
            return False
    return True
```

# 3. Vasya - Clerk.
