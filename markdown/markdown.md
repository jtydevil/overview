# 介绍

markdown是一种纯文本格式的标记语言。
通过简单的标记语法，它可以使普通文本内容具有一定的格式。

## 优点：
1、纯文本，只要支持markdown的地方都能获得一样的编辑效果,方便.
2、操作简单，例如标题样式,markdown只需要在标题内容前加#即可.

# 语法
 
## 一、标题

- 在想要设置为标题的文字前面加#来表示

一个#是一级标题，二个#是二级标题，以此类推。支持六级标题。


  ## 示例：
  
\# 这是一级标题

\## 这是二级标题

\### 这是三级标题

\#### 这是四级标题

\##### 这是五级标题

\###### 这是六级标题

效果如下

# 这是一级标题

## 这是二级标题

### 这是三级标题

#### 这是四级标题

##### 这是五级标题

###### 这是六级标题


## 二、字体
加粗


要加粗的文字左右分别用两个*号包起来

斜体

要倾斜的文字左右分别用一个*号包起来

斜体加粗

要倾斜和加粗的文字左右分别用三个*号包起来

删除线

要加删除线的文字左右分别用两个~~号包起来

示例：

\**这是加粗的文字**

\*这是倾斜的文字*`

\***这是斜体加粗的文字***

\~~这是加删除线的文字~~

效果如下：

**这是加粗的文字**

*这是倾斜的文字*`

***这是斜体加粗的文字***

~~这是加删除线的文字~~

## 三、引用
- 在引用的文字前加>即可。引用也可以嵌套，如加两个>> 三个>>>  n个...

示例：

\ >这是引用的内容

\ >>这是引用的内容


\ >>>>>>>>>>这是引用的内容

效果如下：

- >这是引用的内容

- >>这是引用的内容

- >>>>>>>>>>这是引用的内容

## 四、分割线

三个或者三个以上的 - 或者 * 都可以。

示例：
\---

\----

\***

\*****

效果如下：
可以看到，显示效果是一样的。

---

----

***

*****



## 五、图片

语法：

 ![图片alt](图片地址 ''图片title'')

 图片alt就是显示在图片下面的文字，相当于对图片内容的解释。

 图片title是图片的标题，当鼠标移到图片上时显示的内容。title可加可不加

 上传本地图片直接点击导航栏的图片标志，选择图片即可

## 六、超链接

-语法：

 [超链接名](超链接地址 "超链接title")

 title可加可不加

- 示例：
 \[百度](http://baidu.com)
 
 效果如下：

- [百度](http://baidu.com)

## 七、列表

- 无序列表

- 语法：

- 无序列表用 - + * 任何一种都可以

\- 列表内容

\+ 列表内容

\* 列表内容

注- 意：- + * 跟内容之间都要有一个空格

- 效果如下：

- 列表内容

+ 列表内容

* 列表内容

- 有序列表

 
 语法：
\- 数字加点
\1.列表内容
\2.列表内容
\3.列表内容

- 注意：序号跟内容之间要有空格

- 效果如下：

1.列表内容

2.列表内容

3.列表内容

- 列表嵌套

- 上一级和下一级之间敲三个空格即可

- 一级无序列表内容
 
      1.二级无序列表内容

      2.二级无序列表内容

      3.二级无序列表内容

- 一级无序列表内容

      。二级有序列表内容

      。二级有序列表内容

      。二级有序列表内容

- 一级有序列表内容

      1.二级无序列表内容
   
      2.二级无序列表内容
   
      3.二级无序列表内容

- 一级有序列表内容

      。二级有序列表内容
   
      。二级有序列表内容
   
      。二级有序列表内容

## 八、表格
-语法：
表头|表头|表头

---|:--:|---:

内容|内容|内容

内容|内容|内容

第二行分割表头和内容。

- 有一个就行，为了对齐，多加了几个

文字默认居左

-两边加：表示文字居中

-右边加：表示文字居右

注：原生的语法两边都要用 | 包起来。此处省略

效果如下：

|姓名|技能|排行|
|---|:--:|---:|
|刘备|哭|大哥|
|关羽|打|二哥|
|张飞|骂|三弟|



## 九、代码
语法：
单行代码    
        \`代码内容`

多行代码    
        \```
          代码内容
         ```
效果如下：

单行

create database hero;

多行

function fun(){

  echo "这是一句非常牛逼的代码";

}

fun();

## 十、流程图

```

flow

st=>start: 开始

op=>operation: My Operation

cond=>condition: Yes or No?

e=>end

st->op->cond

cond(yes)->e

cond(no)->op

```




