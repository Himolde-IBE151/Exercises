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

python -m profile program.py
