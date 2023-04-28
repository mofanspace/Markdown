# Markdown基本语法

内容来源：<a href="https://markdown.com.cn/basic-syntax/links.html" target="_blank">Markdown官方教程</a>

## 标题
>使用'#'个数来确定不同大小标题

## 字体
1. **粗体**

`使用**……**编写粗体内容`

2. *斜体*

`使用*……*编写斜体内容`

3. ~~删除线~~

`使用~~……~~编写删除线内容`

4. ***粗斜体***

`使用***……***编写粗斜体内容`

5. 上标<sup>上标</sup>

>例：2<sup>2</sup>

`使用<sup>……</sup>编写上标内容`

6. 下标<sub>下标</sub>

>例：H<sub>2</sub>

`使用<sub>……</sub>编写下标内容`

## 段落

可以通过文本行之间留一个空行来创建新段落。

## 换行符

可以使用`<br>`标签进行换行操作

## 引用文本
> 这是引用文本里的内容

`文本前添加'>'符号`

> 这里是
>
> 多行引用语法：

```
> 这里是
>
> 多行引用语法
```
## 嵌套块引用

快引用可以嵌套。在要嵌套的段落前添加一个`>>`符号

```
> 从前从前
> 有个人爱你很久
>> 但偏偏
>> 雨渐渐
>> 大到我看你不见
```
渲染效果如下：

> 从前从前
> 有个人爱你很久
>> 但偏偏
>> 雨渐渐
>> 大到我看你不见

## 嵌套块的综合运用

块引用可以包含其他Markdown格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。

```
> ### 《晴天》
>
> ————周杰伦<br>
> ***故事的***小黄花
> - 从出生那年就**飘着**
> - 童年的*荡秋千*
>
> 随记忆一直晃到~~现在~~
```
渲染效果如下：

> ### 《晴天》
>
> ————周杰伦<br>
> ***故事的***小黄花
> - 从出生那年就**飘着**
> - 童年的*荡秋千*
>
> 随记忆一直晃到~~现在~~

## 分割线

要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。

```

从前从前

***

有个人爱你很久

---

但偏偏

_____

```
> 效果如下：
>
> 从前从前
>
> ***
>
> 有个人爱你很久
>
> ---
>
> 但偏偏
>
> _____


## 引用代码

1. 单行代码
> 使用单个反引号'`'插入代码块，**前后都需要**。
>为什么会有'前后都需要'，只因例子↓。

例：
`Use git status to list all new or modified  files that haven't yet been committed.`

2. 代码块
>若要将代码或文本格式化为自己的独特块，使用三个反引号'```'，前后都需要。

例：

```
git status
git add
git commit
```
也可以使用每一行缩进至少四个空格或一个制表符，如下：

```
1. 这是一段标签代码
2. 如下：

        <html>
            <head>
                <title>Test</title>
            </head>

3. 如上。

```
效果如下：
1. 这是一段标签代码
2. 如下：

        <html>
            <head>
                <title>Test</title>
            </head>

3. 如上。

## 列表

1. 无序列表
>文字前使用（+、-、*）+ 文本，三个皆可，一块无需列表使用相同符号

```
+ 事件一
+ 事件二
+ 事件三
```
效果如下：

+ 事件一
+ 事件二
+ 事件三

2. 有序列表
> 文字前使用数字(1. )排序

```
1. 任务一
2. 任务二
3. 任务三
```
效果如下：

1. 任务一
2. 任务二
3. 任务三

3. 无序+有序列表
> 注：有序无序均可使用tab键，生成嵌套列表。

```
1. 任务一
    - 事件一
    - 事件二
2. 任务二
    - 事件一
    - 事件二
        1. 计划一
        2. 计划二
        - 意外情况
```
效果如下：

1. 任务一
    - 事件一
    - 事件二
2. 任务二
    - 事件一
    - 事件二
        1. 计划一
        2. 计划二
        - 意外情况

4. 任务列表
>使用`- [ ]`+文本内容
>`- [x]`表示勾选任务框

```
- [x] 学习Markdown语法
    > I am learning.
- [ ] 学习0-1的博客建设
- [ ] 学习游戏开发
```
效果如下：

- [x] 学习Markdown语法
    > I am learning.
- [ ] 学习0-1的博客建设
- [ ] 学习游戏开发

## 表格

Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。

语法格式如下：
```
| 表头 | 表头 |
| ---- | ---- |
| 单元格 | 单元格 |
| 单元格 | 单元格 |
```
效果如下：
| 表头 | 表头 |
| ---- | ---- |
| 单元格 | 单元格 |
| 单元格 | 单元格 |

对齐方式：
+ `:-`表示左对齐。
+ `-:`表示右对齐。
+ `:-:`表示居中对齐。
如下：
```
| 左对齐 | 居中对齐 | 右对齐 | 
| :---- | :----: | ----: |
|   单   |   单   |   单   |
|   单   |   单   |   单   |
```
效果如下：
| 左对齐 | 居中对齐 | 右对齐 | 
| :---- | :----: | ----: |
|   单   |   单   |   单   |
|   单   |   单   |   单   |

## 链接
超链接markdown语法：`[超链接显示名](超链接地址 "超链接title")`

例：

```
+ this site was built using [GitHub Pages](https://pages.github.com)
```

效果为：

+ this site was built using [GitHub Pages](https://pages.github.com)

## 网址和Email地址
使用尖括号可以方便地把URL或者email地址变成可点击的链接。
```
<https://www.baidu.com>

<fake@example.com>
```
效果如下：

<https://www.baidu.com>

<fake@example.com>

## 相对链接
>相对链接是相对于当前文件的链接。例如，如果您在存储库的根目录中有一个自述文件，并且在 docs/CONTRIBUTING.md 中有另一个文件，则自述文件中指向 CONTRIBUTING.md 的相对链接可能如下所示：

`[Contribution guidelines for this project](docs/CONTRIBUTING.md)`

>可以使用所有相对链接操作数，例如 和 。/./../

## 图像 
插入图片markdown语法：`![图片alt](图片链接 "图片title")`

同时也包括统一资源定位符(`url`)和路径(`path`)。
+ 绝对url
> 如果你的图片存储在`GitPage`里面，图片链接格式如下：`https://用户名.github.io/目录名/文件名`

        
        ![这里有一张plmm的照片](https://mofanspace.github.io/images/plmm.jpg "plmm")
        
        
效果如下：

![这里有一张plmm的照片](https://mofanspace.github.io/images/plmm.jpg "plmm")

+ 相对url
> 例如我们gitpage项目里有一个`plmm.jpg`文件，绝对url是：
> 
> `https://github.com/mofanspace/mofanspace.github.io/blob/main/images/plmm.jpg`
> 
> 这个.md文件绝对url是：
> 
> `https://github.com/mofanspace/learn-Markdown/blob/main/README.md`
> 
> 那么，相对url语法如下：

        
        ![这里有一张plmm的照片](../../../mofanspace.github.io/blob/main/images/plmm.jpg "plmm")
        
        
 效果如下：
 
 ![这里有一张plmm的照片](../../../mofanspace.github.io/blob/main/images/plmm.jpg "plmm")

## 图像链接
>图像链接语法：`[![图片alt](图片链接 "图片title")](目标链接url)`

```
[![这里有一张plmm的照片](https://mofanspace.github.io/images/plmm.jpg "plmm")](https://www.baidu.com)
```
效果如下`点击图片跳转至百度`：

[![这里有一张plmm的照片](https://mofanspace.github.io/images/plmm.jpg "plmm")](https://www.baidu.com)
