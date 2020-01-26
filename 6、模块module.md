# 模块module

## module1

```python
# 全局变量
title = "模块1"

# 函数
def say_hello():
    print("我是 %s" % title)

# 类
class Dog(object):
    pass

```

## import导入模块

import module1

module1.title

module1.say_hello

d=module1.Dog()

---------------------------------

import module1 as md1

md1.title

md1.say_hello

d=md1.Dog()

-----------------------------------

from module1 import title;

from module1 import say_hello;

from module1 import Dog;

直接使用

--------------------------------

from module import \*

直接使用

##注意事项

```python
import random
print(random.__file__)
```

输出：

> C:\Users\Hery\Anaconda3\lib\random.py

```
# 全局变量、函数、类，注意：直接执行的代码不是向外界提供的工具！


def say_hello():
    print("你好你好，我是 say hello")


# 如果直接执行模块，__main__
if __name__ == "__main__":
    print(__name__)

    # 文件被导入时，能够直接执行的代码不需要被执行！
    print("小明开发的模块")
    say_hello()
```

## 导入包

包-模块

```python
import hm_message
hm_message.send_message.send("hello")
txt = hm_message.receive_message.receive()
print(txt)
```











