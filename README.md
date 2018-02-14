# 问题猜解
请问你什么时候开始学习前端的？  
比较系统地开始学，大学读了两年半的时候。之前也学过一些。

你觉得你是一个什么样的人？  
比较开朗，能与团队和谐相处；接受新事物的能力比较强；另外比较容易学习新知识。

说一下常见算法的时间复杂度和空间复杂度？  
抱歉，我对此并非很熟悉。但是如果需要实际应用的话，我能从网上找到。

有哪些SEO需要注意的？  
首先是title，description，keywords很重要  
其次语义化html代码  
最后就是不要过度使用React这一类的框架，当然如果是React的ssr就另当别论了

<!doctype>是什么？  
相当于solidate里面的pragma solidate ^4.00。如果说solidate是选择编译器版本，那这个就是选择浏览器解释器版本

语义化好处？  
1、对搜索引擎友好  
2、对开发人员友好

什么是RESTFUL？  
用GET获取资源、用POST更新资源、用DELETE删除资源、用PUT增加资源;用xxx/id/1代替xxx/?id=1；至于好处，除了更加语义化，更装逼外，好像没什么好处；有时候甚至更麻烦

什么情况下会首先发一次Options请求？  
1、跨域  
2、除了POST和GET外的请求  
3、http请求头里面带上自定义参数如access_token

你是怎么理解缓存的？  
1、一般在再一次请求某个资源的时候，会检查Expires是否过期，也会检查是否小于max-age，如果没过期，或者小于max-age，那浏览器直接从缓存里面去，而不去请求服务器（在chrome控制台显示的来源是from disk）  
2、如果上述条件不满足，那么会请求服务器。会发送上次的资源更新时间给服务器，服务器如果检测到未变动，则返回304。浏览器接收304后也从缓存读取

如何优化网站性能？  
1、可变的内容从业务服务器输出，不变的内容从专门存放静态资源的服务器（或者cdn）输出  
2、适当合并静态资源文件，比如常用的小图标做成雪碧图  
3、对于极小的图标，直接base64后放进页面中，可减少http请求次数  
4、使用缓存，尤其是不变性比较高的资源；甚至对于那些变动有规律的资源，也可以采用缓存  
5、尽量将js放到页面底部加载，而将css放到页面顶部加载，防止js阻塞白屏  
6、在网页发布的时候，或者打包的时候，用自动化工具进行代码压缩  
7、对于含有规律的大文件，强烈推荐使用gzip

你用过哪些自动化工具？  
gulp和webpack

怎么清除浮动？  
这种问题不用问了

