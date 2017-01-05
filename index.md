title: 利用NodePPT构建狂拽炫酷吊炸天的PPT
speaker: 刘彪
url: https://huaiyinfeilong.github.io/nodeppt-intro/public/
transition: cards

[slide]

# 利用NodePPT构建狂拽炫酷吊炸天的PPT
## 刘彪
## 2017年1月6日

[slide]

## 什么是NodePPT
---

这可能是迄今为止最好的网页版演示库

* 基于GFM的markdown语法编写
* 支持html混排，再复杂的demo也可以做！
* 支持多个皮肤：colors-moon-blue-dark-green-light
* 实现watch功能nodeppt start -w
* 支持20种转场动画，可以设置单页动画
* 支持单页背景图片
* 多种模式：overview模式，双屏模式，socket远程控制，摇一摇换页，使用ipad/iphone控制翻页更酷哦~
* 可以使用画板，双屏同步画板内容！可以使用note做备注
* 支持语法高亮，自由选择highlight样式
* 可以单页ppt内部动画，单步动画
* 支持进入/退出回调，做在线demo很方便
* 支持事件update函数，查看demo

[slide]

## 样例展示

双屏控制： http://qdemo.sinaapp.com/?_multiscreen=1

手机百度前端之路：http://qdemo.sinaapp.com/box-fe-road.htm 

[slide]

## 环境配置
---

### 安装NodeJS

Node.js中文网下载对应版本安装：

http://nodejs.cn/download/

### 安装NodePPT

```
npm install -g nodeppt
```

[slide]

## 必备的Markdown语法
---

### 标题

标题由“#”开头，“#”一个“#”代表一级标题，“##”两个“#”代表二级标题，以此类推。

### 代码

代码块以“```”开头，同样也以“```”结尾。

### 列表

无序列表的列表项目钱加“-”“+”或“*”，有序列表的列表项钱加“1. …… n.”，也可全部为“1.”，实际上有序列表的显示并不使用Markdown源码中的数字，而是紧紧需要数字来表示有序而已。

更多Markdown语法可参见《Markdown语法说明（简体中文版）》：

http://wowubuntu.com/markdown/

[slide]

## 创建第一个PPT
---

```
nodeppt create PPT文件名（无需扩展名，默认添加.md扩展名）
```

[slide]

## NodePPT语法
---

### 重要语法

title:标题

speaker：演讲者

url：URL

[slide]

transition:转场效果，推荐cards，对无障碍支持好。可选的转场效果有：

* kontext
* vkontext
* circle
* earthquake
* cards
* glue
* stick
* move
* newspaper
* slide
* slide2
* slide3
* horizontal3d
* horizontal
* vertical3d
* zoomin
* zoomout
* pulse

[slide]

方括号slide：换页

### 更多语法

想要获取NodePPT的更多帮助信息，可上网查阅或浏览以下位置的Demo官方样例：

C:\Users\Administrator\AppData\Roaming\npm\node_modules\nodeppt\ppts

[slide]

## NodePPT效果预览
---

```
nodeppt start -d ppt所在目录 -p 端口号
```

[slide]

## PPT导出
---

### HTML导出

导出全部，包含css、js、img，默认在publish文件夹：

```
nodeppt generate MD文件名 -a
```

导出全部，包含css、js、img，指定存放文件夹：

```
nodeppt generate MD文件名 导出路径 -a
```

### 导出PDF

Chrome浏览器，URL末尾追加“print=1”后，Ctrl+P打印，选择导出PDF。

[slide]

## 亲自试一试
---

你心动了吗？心动不如行动，亲自试一试吧！
