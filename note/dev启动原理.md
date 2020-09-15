dev分两种，一种是直接的dev，一种是dev:play

dev的入口文件是`examples/entry.js`

dev:play的入口文件是`examples/play.js`

这两种其实可以理解为都是一个vue项目。



**关于路由**

play模式没有路由，或者说路由就是自己的play页面

dev模式有路由，路由比较复杂，复杂是因为要适配i18n



**编译md文件**

大家可以发现其实有些路由是引入md文件的，而不是vue文件。其实价格loader就可以了。

element这里用的是`markdown-it-chain`这个loader



【TODO】

1. dev:extension命令