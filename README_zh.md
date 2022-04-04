# 100以内随机数的求和挑战

挑战写出最快的求和算法，把2个0~99之间的自然数加起来。

## 游戏规则

本挑战的目标是一段能够不停地随机取2个0~99之间的自然数并将它们加起来的代码（例如：随机取16和70，16+70=86）。程序不能抛出异常或有bug（你要确保你的代码能够运行，且运算结果正确）。每完成一次求和，计数1次。

例如下面这段Python代码（这显然不是一个好答案，帮助理解）：

```python
from random import randint
from time import time

current_time = time()
count = 0

# 计时开始
while time() - current_time < 1:
    a = randint(0, 99)
    b = randint(0, 99)
    c = a + b
    count += 1
# 计时结束

print(count) # 输出完成计算的次数
```

允许使用任何语言编写，只要算法是对的。除了计算方面，你可能还需要考虑选随机数的效率。

你需要创建一个目录并把代码装进目录里。你的代码必须刷新这里的记录（以你的机器为标准，我们会确认），还可以来点刺激的，比如手写语言或者改良编译器之类的操作，本挑战均允许。

------

If you have any question or suggestion for the game rules, create an [issue](https://github.com/rice0208/ranint-sum-challenge/issues).