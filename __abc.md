# abc模块

## abc模块是一个提供编写抽象类的工具的模块


1. `abstractmethod`
作用：普通方法装饰器
原理：为方法添加了一个`__isabstractmethod__=True`的属性
用法：```
     @abstractmethod
     def my_abstract_method(self, ...):
         ...
     ```

2. `abstractclassmethod`
作用：类方法装饰器
原理：为方法添加了一个`__isabstractmethod__=True`的属性
用法：```
     @abstractclassmethod
     def my_abstract_classmethod(self, ...):
         ...
     ```

3. `abstractstaticmethod`
作用：静态方法装饰器
原理：为方法添加了一个`__isabstractmethod__=True`的属性
用法：```
     @abstractstaticmethod
     def my_abstract_staticmethod(self, ...):
         ...
     ```

4. `abstractproperty`
作用：属性函数property装饰器
原理：为方法添加了一个`__isabstractmethod__=True`的属性
用法：```
     @abstractproperty
     def my_abstract_property(self, ...):
         ...
     ```
注意：该装饰器已经弃用，应该用property+abstractmethod代替

5. `ABCMeta`
作用：定义抽象类的元类，核心类
