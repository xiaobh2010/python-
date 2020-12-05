# python-
----------------------------------------------------------------------------
类方法
（1）定义
@classmethod
def 方法名称(cls,参数列表):
  方法体

（2）调用：
类名.方法名(参数列表)


class YYY:
    total=100
    def __init__(self):
        YYY.total-=1

    @classmethod
    def print_total(cls):
        print(cls.total)
y=YYY()
YYY.print_total()


----------------------------------------------------------------------------
静态方法
1 定义
@staticmethod
def 方法名称(参数列表):
  方法体

2 调用
类名.方法名(参数列表)
不建议通过对象访问静态方法


class XXX:
    def __init__(self):
        pass
    @staticmethod
    def func():
        print('hello world')
x=XXX()
XXX.func()


----------------------------------------------------------------------------
super（）方法
示例：
class Animal:
    def __init__(self,name,age=0):
        self.name=name
        self.__age=age

class Dog(Animal):
    def __init__(self,name,age,score=0):
        super().__init__(name,age)
        self.score=score












































