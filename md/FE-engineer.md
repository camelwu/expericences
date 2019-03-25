## 前端是一种GUI软件
现如今前端可谓包罗万象，产品形态五花八门，涉猎极广，什么高大上的基础库/框架，拽炫酷的宣传页面，还有屌炸天的小游戏……不过这些一两个文件的小项目并非是前端技术的主要应用场景，更具商业价值的则是复杂的Web应用，它们功能完善，界面繁多，为用户提供了完整的产品体验，可能是新闻聚合网站，可能是在线购物平台，可能是社交网络，可能是金融信贷应用，可能是音乐互动社区，也可能是视频上传与分享平台……  
> 从本质上讲，所有Web应用都是一种运行在网页浏览器中的软件，这些软件的图形用户界面（Graphical User Interface，简称GUI）即为前端。  

如此复杂的Web应用，动辄几十上百人共同开发维护，其前端界面通常也颇具规模，工程量不亚于一般的传统GUI软件：  

![alt](./static/web_gui.png)  

尽管Web应用的复杂程度与日俱增，用户对其前端界面也提出了更高的要求，但时至今日仍然没有多少前端开发者会从软件工程的角度去思考前端开发，来助力团队的开发效率，更有甚者还对前端保留着”如玩具般简单“的刻板印象，日复一日，CV大法刀耕火种。  

网站开发（asp、php、jsp等不分离）->前后分离（简单构建）->工程、模块化开发，技术已经日新月异，学不动也要学。

### 前端工程的三个阶段
现在的前端开发倒也并非一无所有，回顾一下曾经经历过或听闻过的项目，为了提升其前端开发效率和运行性能，前端团队的工程建设大致会经历三个阶段：
#### 第一阶段：库/框架选型

前端工程建设的第一项任务就是根据项目特征进行技术选型。  
js：prototype，mootools，jQuery，bootstrap，underscore+backbone，zepto，knockout，angular，react，vue  
css：animate.css，normalize.css  

基本上现在没有人完全从0开始做网站，哪怕是政府项目用个jquery都很正常吧，React/Angularjs等框架横空出世，解放了不少生产力，合理的技术选型可以为项目节省许多工程量这点毋庸置疑。  

#### 第二阶段：简单构建优化

选型之后基本上就可以开始敲码了，不过光解决开发效率还不够，必须要兼顾运行性能。前端工程进行到第二阶段会选型一种构建工具，对代码进行压缩，校验，之后再以页面为单位进行简单的资源合并。  

grunt，gulp 对资源进行压缩合并和打包，当然，这两个技术已经更新换代很久，只是现在使用的人不多了。  

#### 第三阶段：JS/CSS模块化开发

namespace方式，requireJs，seaJs，webpack，less，sass可以看到前端模块化技术的演进之路，从Yahoo最早提出命名空间开始，到AMD|CMD模块开发，到目前最常接触到的webpack。  

分而治之是软件工程中的重要思想，是复杂系统开发和维护的基石，这点放在前端开发中同样适用。在解决了基本开发效率运行效率问题之后，前端团队开始思考维护效率，模块化是目前前端最流行的分治手段。  

> 很多人觉得模块化开发的工程意义是复用，我不太认可这种看法，在我看来，模块化开发的最大价值应该是分治！分治！分治！  

不管将来是否要复用某段代码，请将其分治为一个模块。  

现在Js模块化方案很多，AMD|CMD/CommonJS/UMD/ES6 Module等，对应的框架和工具也一大堆，说起来很烦，大家自行百度吧；CSS模块化开发基本都是在less、sass、stylus、postcss等预处理器的import/mixin特性支持下实现的。

#### 第四阶段

前端是一种技术问题较少，工程问题较多的软件开发领域；很多工程化方式都是从后端或软件工程中借鉴过来的。当我们要开发一款完整的Web应用时，前端将面临更多的工程问题，比如：  

大体量：多功能、多页面、多状态、多系统；
大规模：多人甚至多团队合作开发；
高性能：CDN部署、缓存控制、文件指纹、缓存复用、请求合并、按需加载、同步/异步加载、[移动端骨架屏](http://gitlab.lvyuetravel.com/camel/technology-share/blob/master/md/skeleton-content-loader.md)、HTTP 2.0服务端资源推送。
> 进阶阅读：  
[怎样开发和部署前端代码？](http://gitlab.lvyuetravel.com/camel/technology-share/blob/master/md/version.md)   
[适用旅悦的简单方案](http://gitlab.lvyuetravel.com/camel/technology-share/blob/master/md/dist2compress4push.md) 

前面讲的三个阶段虽然相比曾经“茹毛饮血”的时代进步不少，但用于支撑第四阶段的多人合作开发以及精细的性能优化，还需经历一系列工程问题。