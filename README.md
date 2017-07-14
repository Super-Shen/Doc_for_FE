## 前端技术文档

### 1. 技术方案

#### 1.1. 基础知识

- html

- css

- javascript（ECMAScript5）

- Coffeescript

#### 1.2. 开发工具

##### 1.2.1. 编辑器
- sublime
- webstorm

##### 1.2.2.调试工具
- Chrome Dev Tools

##### 1.2.3.自动化及包管理工具
- npm
- Grunt

#### 1.3.前端框架（库）

- jQuery
- Bootstrap
- Echarts
- *Express

#### 1.4.其他技术

- nodejs
- Ajax
- 建议使用Markdown标记语言撰写文档

### 2.技术规范

#### 2.1.通用规范

- CSS样式属性或者javascript代码后加“;”
- 文件内容编码均统一为UTF-8。
- 文件名用英文单词，全部采用小写方式， 多个单词用下划线分隔。

#### 2.2.Html规范

- 嵌套的节点应该缩进，缩进使用TAB键或使用4个空格。
- 在属性上，使用双引号，不要使用单引号。
- 不要在自动闭合标签结尾处使用斜线，不要忽略可选的关闭标签。
- 在页面开头使用这个简单地doctype来启用标准模式，使其在每个浏览器中尽可能一致的展现；编码统一为UTF-8。
``` markdown
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
    </head>
    ...
</html>
```
- 在<head>中添加详细信息。
``` markdown
<meta name="author" content="smile@kang.cool">//作者
<meta name="description" content="hello">//网页描述
<meta name="keywords" content="a,b,c">//关键字,“，”分隔
<meta http-equiv="Window-target" content="_top">//用来防止别人在框架里调用你的页面
<meta http-equiv="Refresh" content="5;URL=http://kahn1990.com/">//跳转页面，5指时间停留5秒 网页搜索机器人向导。用来告诉搜索机器人哪些页面需要索引，哪些页面不需要索引
<meta http-equiv="X-UA-Compatible" content="IE=Edge">
```
- 非特殊情况下CSS样式文件外链至<head>之间，javascript 文件外链至页面底部.通常在引入css和js时不需要指明 type，因为 text/css 和 text/javascript 分别是他们的默认值。
``` markdown
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="css/index.css">
</head>
<body>
    ···
    <script src="jquery/jquery-2.1.1.min.js"></script>
</body>
</html>
```
- 属性应该按照特定的顺序出现以保证易读性；
    class
    id
    name
    data-*
    src, for, type, href, value , max-length, max, min, pattern
    placeholder, title, alt
    aria-*, role
    required, readonly, disabled
- 语义化HTML，且尽可能减少<div>嵌套。
#### 2.3.css规范
- 每个属性声明末尾都要加分号。
- CSS书写顺序。
``` markdown
.header {
/* 显示属性 */
    display || visibility
    list-style
    position top || right || bottom || left
    z-index
    clear
    float
/* 自身属性 */
    width max-width || min-width
    height max-height || min-height
    overflow || clip
    margin
    padding
    outline
    border
    background
/* 文本属性 */
    color
    font
    text-overflow
    text-align
    text-indent
    line-height
    white-space
    vertical-align
    cursor
    content
    };
```
- 空行：文件最后保留一个空行；'}'后最好跟一个空行；不同类的属性之间。

- 需要空格：

  - 属性值前
  - 选择器'>', '+', '~'前后
  - '{'前
  - `!important` '!'前
  - 属性值中的','后
  - 注释'/*'后和'*/'前

- 不需要空格：

  - 属性名后
  - 多个规则的分隔符','前
  - `!important` '!'后
  - 属性值中'('后和')'前

- 换行：

  - '{'后和'}'前
  - 每个属性独占一行
  - 多个规则的分隔符','后
  - '{'前 不换行！！！

- 命名：类名使用小写字母，以中划线分隔，id采用驼峰式命名。

### 3.学习路径
- 当你在浏览器中输入google.com并按下回车后发生了什么 https://github.com/skyline75489/what-happens-when-zh_CN
#### 3.1.html
- HTML+CSS基础课程 http://www.imooc.com/learn/9
- MDN的HTML入门 https://developer.mozilla.org/zh-CN/docs/Web/HTML
- 网页简单布局之结构与表现原则 http://www.imooc.com/learn/20
#### 3.2.css
- HTML+CSS基础课程 http://www.imooc.com/learn/9
- 如何用CSS进行网页布局 http://www.imooc.com/learn/57
- MDN的CSS入门教程 https://developer.mozilla.org/zh-CN/docs/Web/CSS
- 学习CSS布局 http://zh.learnlayout.com/display.html
#### 3.3.javascript
- JavaScript入门篇 http://www.imooc.com/learn/36
- JavaScript菜鸟教程 http://www.runoob.com/js/js-tutorial.html
#### 3.4.jQuery
- jQuery基础 （一）-（三）http://www.imooc.com/course/list?c=jquery&is_easy=1
- jQuery菜鸟教程 http://www.runoob.com/jquery/jquery-tutorial.html

#### 3.5.bootstrap
- bootstrap基础 http://www.imooc.com/learn/141
- bootstrap官方文档 http://v3.bootcss.com/

For more: http://html5ify.com/fks/
