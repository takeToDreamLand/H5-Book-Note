# 《HTML5H5基础知识、核心技术以及前沿案例》学习笔记

> [目录]
>> [第一部分 HTML5基础](#第一部分-HTML5基础)
>>> [第1章 初探HTML5](#第1章-初探HTML5) 
  | [第2章 HMTL5新手详解](#第2章-HMTL5新手详解)
  | [第3章 CSS3新手详解](#第3章-CSS3新手详解)
  | [第4章 JavaScript新手详解](#第4章-JavaScript新手详解)
  | [第5章 移动端HTML5开发详解](#第5章-移动端HTML5开发详解)
  | [第6章 事半功倍：运用流行开源类库](#第6章-事半功倍：运用流行开源类库)
  | [第7章 HTML5与周边编程语言、软件](#第7章-HTML5与周边编程语言、软件)
>> [第二部分 HTML5前沿经典应用篇](#第二部分-HTML5前沿经典应用篇)
>>>[第8章 HTML5页面元素与布局](#)
  | [第9章 HTML5动画与动效](#)
  | [第10章 HTML5图形和图像](#)
  | [第11章 HTML5交互操作](#)
  | [第12章 HTML5页面组件](#)
  | [第13章 HTML5音频与视频](#)
  | [第14章 HTML5响应式设计](#)
>>>
  | [](#)

## 第一部分 HTML5基础
### 第1章 初探HTML5
1. 通过将`html`元素的`height`设为`100%`来使内容（比如背景）自适应窗口。

2. 背景调整可以通过上一条笔记以及将`background-size`属性设为`cover`来使背景铺满页面；
并且可以将`background-position`设为`center`来使背景以页面中心为原点（而不是左上角）。

3. 由于使用`H1`标题，其自带的`padding`顶出了父元素（尤其在父元素设置`margin`为`0`时），如下：
![页面][1]

4. 伪元素介绍

    | 属性          | 描述                             | CSS |
    |---------------|----------------------------------|-----|
    | :first-letter | 向文本的第一个字母添加特殊样式。 | 1   |
    | :first-line   | 向文本的首行添加特殊样式。       | 1   |
    | :before       | 在元素之前添加内容。             | 2   |
    | :after        | 在元素之后添加内容。             | 2   |

5. 对象居中的实现方法：首先将对象的**父元素**（比如**body**或**html**）的`position`属性设为`relative`，接着将对象的`margin-top`属性设为`50%`（或`margin: 50% 0 0 0`），之后将`transform`属性设为`translateY(-50%)`，如果使用这个方法，需要处理浏览器兼容的问题。整体代码如下：
    ```css
    #container {
        width: 100%;
        text-align: center;
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        -moz-transform: translateY(-50%);
        -ms-transform: translateY(-50%);
        -webkit-transform: translateY(-50%);
        -o-transform: translateY(-50%);     
    }
    ```

### 第2章 HMTL5新手详解

1. 页面根元素`html`：







[1]: imgs/img1.png