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
URI Online Judge | 1168

John wants to set up a panel containing different numbers of LEDs. He does not have many leds, he is not sure if he will be able to mount the desired number. Considering the configuration of the LEDs of the numbers below, make an algorithm that helps John to discover the number of LEDs needed to set the value.

#### Input
The input contains an integer N, (1 ≤ N ≤ 2000) corresponding to the number of test cases, followed by N lines, each line containing a number (1 ≤ V ≤ 10100) corresponding to the value that John wants to set with the leds.
Output

For each test case, print one line containing the number of LEDs that John needs to set the desired value, followed by the word "leds".
Input Sample 	Output Sample

|3 |  |  
| :---: | :---: |
|115380   |  27 leds|
|2819311  |  29 leds|
|23456    |  25 leds|

Solution:
```python
# input: an integer N (number of test cases)
#        followed by N lines, each line containing an integer V (the value that John wants to set with the leds)
# output: For each test case, one line containing the number of LEDs that John needs to set the desired value, followed by the word "leds"
# The leds for each number may be defined as:
# led_list = [6, 2, 5, 5, 4, 5, 6, 3, 7, 6]
# where lef_list[0] is the amount of leds necessary to represent the number 0 in the panel.
# As in many URI exercises, the solution consists in iterating through all the N test cases and execute a computation for each test case:
N = int(input())
for n in range(N):
    V = input()
    print(how_many(V))
```
How would you implement the function how_many(V), that receives a word and returns the amount of leds necessary to represent it in the panel?


