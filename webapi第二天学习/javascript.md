# Bom对象

## 1.location

### 常用属性：

1. `href`：用于跳转页面
2. `url`:获取url后面的请求参数
3. `hash`:获取url中#和后面的参数

### 常用方法

1. reload：

   ```
   location.reload(`boolean`)
   ```

   

## 2.navigator

## 3.history

### 常用方法

1. ```javascript
   history.back() //后腿
   ```

2. ```javascript
   history.forword() //前进
   ```

3. ```javascript
   history.go('num') //前进num步
   ```

   

## 4.localStorage和sessionStorage

### 基本方法

```javascript
 //存储,本地存储只能存字符串
    localStorage.setItem(`name`, `张三`)
    localStorage.setItem(`age`, `18`)
//删除
    localStorage.removeItem('name')
//获取本地存储，注意是以字符串的方式返回
localStorage.getItem('age')
```

#### 存储对象

```javascript
const obj = {
      user: 'jone',
      sex: 'nan',
    }
    localStorage.setItem('obj', JSON.stringify(obj))
    console.log(localStorage.getItem('obj'))
```

需要使用JSON.stringify(obj)方法使对象转化为json对象

#### 取json对象

```
JSON.parse()
```

# 数组方法

```javascript
let arr = ['张三', '李四', '王五']
//map方法对数组每一个元素进行操作
    let arr1 = arr.map(function (item, index) {
      return '名字:' + item
    })
    console.log(arr1);
//join方法使数组拼接成字符串
    let newarr = arr1.join()
    console.log(newarr);
```

# 正则表达式

## 1.使用步骤

```javascript
let texct = '我是一只猫，快乐的星猫'
//定义规则
const rule = /猫/
    //匹配
console.log(rule.test(texct))
rule.exec(texct)//返回数组
```

## 元字符

![image-20231107220543069](C:\Users\张吉勇\AppData\Roaming\Typora\typora-user-images\image-20231107220543069.png)

> 如果^和$同时使用表示使用的是精确匹配

实例，账号只能6-18位，且只能由英文字母，__和数字构成

```javascript
/^[A-z0-9-_]{6,18}$/
```

