# 介绍
Element Plus是Element UI开源项目的升级版。就是基于VUE3重新开发了Element UI。

因为Element UI是基于VUE2开发的。

而VUE3和VUE2并不兼容。

Element Plus是一套桌面端组件库，提供了很多基于VUE3开发的组件，方便用户开发炫酷的Web应用。



Element Plus官方写了一个初学者工具包element-plus-starter。

用户可以直接git clone这个项目，然后就可以使用Element Plus和Vue3进行前端页面开发了。

然而，这个初学者工具包对于我来说不是很好用，因此我基于这个项目，

重新写了一个typescript的初学者工具包。





# element-plus-starter-ts项目介绍
基于element-plus-starter，我为Element Plus重写的支持typescript的初学者工具包命名为element-plus-starter-ts。

这个项目比官方的element-plus-starter项目多了两个功能：



1. 支持TypeScript

现在在前端开发领域，typescript是很流行的。因为JavaScript的并行版本太多，浏览器不兼容。

TypeScript会通过编译为对应版本的JavaScript的方式，解决这些恼人的问题。使用TypeScript不用管浏览器，都可以使用比较新的JavaScript语法。

Vue3也是使用TypeScript开发的。

所以，我觉得应该为使用TypeScript开发的朋友提供Element Plus的初学者工具包。



2. 支持相对路径部署
   

官方的element-plus-starter项目，在部署时，必须被部署到服务器的根目录下。而这在现实中是很难做到的。

因为一个Web服务器只有一个根目录。但是，我们服务器上部署的网页数量可能是非常多的。

因此，element-plus-starter-ts项目支持相对路径。你可以把dist目录复制到任意Web服务器的任意路径下，照样能工作。

适合实际的部署环境。



# element-plus-starter-ts项目的正确打开方式
element-plus-starter-ts项目的正确打开方式如下：



1. 打开element-plus-starter-ts项目主页。



2. 在命令行中执行如下代码：
   
`
git clone https://github.com/shendl1978/element-plus-starter-ts.git

cd ./element-plus-starter-ts

npm install
`

 这样操作后，你就在本地有了一个支持TypeScript的Element Plus项目了。



3. 再打开一个新的命令行窗口，执行如下代码：
   
`
tsc -w
`

现在，你编写任何typescript代码，都会被即可编译为javascript文件。



4. 要测试写好的网页，在命令行中执行如下代码：
   
`
npm run serve
`

nodejs服务器完成启动后，浏览器中打开 http://localhost:8080/index.html 即可看到开发好的页面。



5. 生成可部署的网页。需要在命名行中执行如下代码：


`
npm run build
`

完成后，把dist目录复制到Web服务器下的对应目录下，即完成了Element Plus网页的部署。



# 总结
Element Plus的支持TypeScript的初学者工具包element-plus-starter-ts比官方的element-plus-starter项目多了两个功能：支持TypeScript和相对路径部署。

希望对读者有所裨益。



