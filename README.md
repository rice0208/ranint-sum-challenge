# Random-int Sum Challenge

Try to make the fastest code adding 2 integers from 0 to 99 together!

## Rules

The target of the challenge is to write a piece of code, which can continuously calculate the sum of 2 integers from 1 to 99 (e.g. 16+70=86). The program must be able to run without bugs, which means you must verify your algorithm to make sure there is no wrong answer. Every time a calculation is finished, the count is added by 1. All the calculations are made within 1 second.

For example (Python, of course this is not the best solution):

```python
from random import randint
from time import time

current_time = time()
count = 0

# 1-sec timer starts
while time() - current_time < 1:
    a = randint(0, 99)
    b = randint(0, 99)
    c = a + b
    count += 1
# timer stops

print(count) # the count of calculations
```

The code can be written in any language (even Brainfuck or something else, only if your algorithm is right). Note that the calculations can be made into other forms.

**Tips** Besides the addition calculation, how to pick a random number is also important.

Fork, make a new directory, and put your code in it to upload your code. Every time the code must be a new record, for example, if the current record of count is 1,000,000 in your place, your code must be more than 1,000,000. Of course you can write a language or better interpreter by yourself.

Good luck.

------

If you have any question or suggestion for the game rules, create an [issue](https://github.com/rice0208/ranint-sum-challenge/issues).