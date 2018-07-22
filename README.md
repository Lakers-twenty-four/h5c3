# HTML5 #

## 1.1 介绍 ##

[百度百科](https://baike.baidu.com/item/html5/4234903)

&emsp;&emsp;HTML5是HTML4的升级版

&emsp;&emsp;HTML5新增了和优化了
- 新的语义化标签
- 本地存储功能
- 多媒体功能
- 画布功能
- 新的javascript的API
- 浏览器本地应用功能
- CSS3

&emsp;&emsp;日常我们所说的HTML5其实就是一个统称，他其实包含了

> HTML5 = 新的标签 + css3 + 新的javascript API

H5第一天

- 理解

    - 理解和使用盒子模型的內减模式
    - 理解和设置常见边框圆角
    - 掌握线性渐变的设置
    - 理解和使用过渡属性实现常见效果
    - 理解和使用2d转换实现常见效果

## 內减模式 ##
- 在CSS3中，计算盒子宽度的方式分为两种：1 传统模式 2 內减模式

- 两者的区别主要是体现在计算元素的宽度或者高度的方式上。通过 box-sizing 属性来控制


> #### 传统模式 #####

- 我们一直在写的元素的盒子模型，默认就是传统模式  box-sizing: content-box;

- 盒子的宽度计算方式为：

    - 传统模式 宽度计算 ： 盒子的宽度 = css中设置的 width + border +padding
    - 內减模式 宽度计算 ： 盒子的宽度  = css中设置的宽度 width 属性值为 boder-box

![](./mdImg/內减模式2.png)

> ### 內减模式 ###
![]("https://github.com/Lakers-twenty-four/h5c3/blob/master/mdImg/%E5%85%A7%E5%87%8F%E6%A8%A1%E5%BC%8F1.png")
- 观察得出： 內减模式的特点
    - 元素真实的宽度就是css中设置的宽度
    - 当css中的width定好了之后，动态的改变border或者padding，只有内容的宽度见减少

- 应用场景
    - 常用在样式的初始化中，避免一个像素之差导致的布局换行

![]("https://github.com/Lakers-twenty-four/h5c3/blob/master/mdImg/%E5%85%A7%E5%87%8F%E6%A8%A1%E5%BC%8F3.png")