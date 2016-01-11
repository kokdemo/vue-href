# vue-href
a simple way to write href for every dom in vue.js

###Any English description here?

sorry, I will add English version description soon.

###这是啥？

一个vue.js的指令插件，可以让你给任何dom加上一个跳转的事件。
属于那种并没有什么卵用但是写起来还蛮省事的插件。

###有啥用？

你原来可能需要这样写一个跳转：

    <a href='http://google.com'><h1>点我</h1></a>
    
现在：

    <h1 v-href="'http://google.com'">点我</h1>


###怎么用？

直接引入vue-href.js，将来可能会写一些更优雅的方式，目前嘛，我懒。
你可以下载repo，然后看一下demo下面是怎么写的。

###花式玩法？

新窗口打开：

    <div id="demo2" v-href:blank="'http://google.com'">
        click me to open new tab to google
    </div>
    
还可以这么写：

    v-href:b
    v-href:blank
    v-href:new
    
原窗口跳转：

    v-href
    v-href:o
    v-href:origin
    
###一些回调函数？

也是有的，你需要这么写：
    
    v-href="[url,before,after]"
    
before和after分别会在跳转前后执行。
