# Exercises


```python
try:
    my_file = open(filename, "r")
except FileNotFoundError:
    print('File not found, creating one')
    my_file = open(filename, 'w')
    my_file.write("A first line\n")
    #print("A first line", file = my_file)
else:
    line = my_file.readline()
    print("first line", line)
finally:
    my_file.close()
```

## Exercises on sequences
Alarm Clock URI Online Judge | 1103

## Exercises on sequences
URI Online Judge | 1068

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

Highest and Position URI Online Judge | 1080
?


Search
```python
def search_elem(L, key):
    for num in L:
      if num == key:
          return True
    return False

print(search_elem([1, 10, 20, 30, 50, 100], 30))
```
