# Exercises
This is an unfinished solution for the URI 1168 problem. What do you think it needs to be finished?
```python
N = int(input())
for n in range(N):
    V = input()
    print(how_many(V))

def how_many():
    total = 0
    for each p in word:
        total = total + leds(p)

def leds(p):
    led_list = [6, 2, 5, 5, 4, 5, 6, 3, 7, 6]
    return led_list[p]
```
```python
def search_elem(L, key):
    for num in L:
      if num == key:
          return True
    return False

print(search_elem([1, 10, 20, 30, 50, 100], 30))
```

```python
python -m profile program.py
```

```python
try:
    file = open(filename)
    new_filename = file.readline()
except FileNotFoundError:
    print('File not found, creating one')
    file = open(filename, 'w')
else:
    new_file = open(new_filename)
    data = new_file.read()
finally:
    file.close()
```
