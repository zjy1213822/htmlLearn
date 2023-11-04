# 事件备忘录

## 1.鼠标事件

1. 对于鼠标事件使用`mouseenter`和`mouseleave`,而不轻易使用`mouseover`和`mouseout`防止冒泡

2. 事件冒泡

   微软提出了名为事件冒泡(event bubbling)的事件流。事件冒泡可以形象地比喻为把一颗石头投入水中，泡泡会一直从水底冒出水面。也就是说，事件会从最内层的元素开始发生，一直向上传播，直到document对象，结果使子类会使用到父类的方法。

## 2.事件对象的一些属性和方法

- ![image-20231104164124369](C:\Users\张吉勇\AppData\Roaming\Typora\typora-user-images\image-20231104164124369.png)
- ![image-20231104164147446](C:\Users\张吉勇\AppData\Roaming\Typora\typora-user-images\image-20231104164147446.png)

1. 阻止冒泡：`当前对象.stopPropagation()`
2. 阻止网页默认行为：`e.preveDefault()`

## 3.鼠标滚动事件

![image-20231105004501082](C:\Users\张吉勇\AppData\Roaming\Typora\typora-user-images\image-20231105004501082.png)

### 3.1相关属性

![image-20231105004951933](C:\Users\张吉勇\AppData\Roaming\Typora\typora-user-images\image-20231105004951933.png)

![image-20231105010106840](C:\Users\张吉勇\AppData\Roaming\Typora\typora-user-images\image-20231105010106840.png)