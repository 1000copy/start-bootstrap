

#介绍

bootstrap是Twitter公司出品的css框架，被前端程序员欣赏并广为采用。那么它给web网页带来了什么呢。我们从一个按钮的样式开始。假设如下代码的网页，页面内只有一个按钮：

    //normal.html
    <!DOCTYPE html>
    <html >
      <head>
        <title>Bootstrap</title>
      </head>
      <body>
        <button>Hello</button>
      </body>
    </html>

当使用浏览器查看时:

    open normal.html

网页和按钮的外观是浏览器默认提供的。普通而平凡。

然而，当我们引入bootstrap，同样的按钮看起来就有声有色了。至少相当一部分采用了此框架的人是这样看的。

    // bootstrap.html
    <!DOCTYPE html>
    <html >
      <head>
        <title>Bootstrap</title>
        <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
      </head>
      <body>
        <button class="btn">Hello</button>
      </body>
    </html>

请打开浏览器查看如下的文件：
    
    open bootstrap.html

对比下两个html文件，可以看到，魔术的变化来自于：

1. 多出来了一个css文件的引入，此文件位于bootstrap的cdn服务器上，这样就暂时不必自己下载bootstrap套件，即可看到效果了。
2. bootstrap的链接是 https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css
3. 对指定的button元素，应用class，值为btn

bootstrap的大部分效果的应用来自于对class属性的操纵。比如我们可以继续把button改造出各种样子来，一时间，百花齐放：

    <button class="btn">Hello</button>
    <button class="btn btn-primary">Hello</button>
    <button class="btn btn-success">Hello</button>
    <button class="btn btn-info">Hello</button>
    <button class="btn btn-warning">Hello</button>
    <button class="btn btn-danger">Hello</button>

我们很多人知道，样式起了作用，秘密在于bootstrap.css文件，但是有了此文件，我们甚至不必深入了解css是什么，以及如何做到这样的效果；而只要修改class属性的值，就可以得到各种为人称道的页面展示了。

实际的效果，可以在此处：https://jsfiddle.net/1000copy/e7a32w9y/ 看到。这个网站可以让我们不必写很多html的head和body标签，并且在一屏内同时编写js、html、css，并展示最终网页的效果。


## 分类法

Bootstrap主要有数十个组件构成。一般来说，目前是罗列所有的组件，逐一的讲解它的外观、class、数据属性（data-*前缀属性）等。这样不容易理解各个组件的关系，也无法知道Bootstrap的封装逻辑。

本小书会根据Bootstrap改造的标签做出分类，分为若干组。比如对ul的改造而来的若干组件构成一个组，这个组为list类。所有基于ul的Bootstrap组件分为一类，集中讲解。这样做的好处，就是可以对照原生HTML元素的外观和被Bootstrap改造后的外观，以及改造的方法。这样的组织体例是读者而言是更加容易理解的方式。列表为分类后的组件清单：

这样分类并不都是那么科学和准确的。比如Bootstrap Panel组件是常常用来改造div标签，因此被归入div类。但是如果不使用div，而是使用nav，也一样可以达到类似的效果。但是这样做确实简化了分类的方式，也节省了读者的理解成本。

本小书把对div的改造分类一个类叫做div类。以此类推，还有span类、ul类、button类、img类、form类、input类。随后是高级类别的组件，分别是dropdown、jumbotron、carousel、navbar、popup。最后讲解Bootstrap布局。

随后章节，以此结构展开。








    
