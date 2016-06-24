---
title: 就是任性：用JavaScript开发APP！
date: 2016-06-11 16:54:05
tags: 美文转载
---

**（写在前面的前面）**

有时候这人就是贱，非要虐的自己死去活来才安心，那么我就分享分享这好几个下午一坐就是四五个小时的我

————都`干`了什么。

![暴漫](https://raw.githubusercontent.com/jeasonstudio/images/749c8168af9dea6b6318b2672ceb5f123097950b/20160611/bmzb.jpg)

 * 搞了搞前端，就会有种很不爽的感觉，总被人说成是美工，而且现在搞前端烂大街。
 * 经常被人问到，你是不是会写APP啊————不想跟连网站跟APP都分不清的人解释（请不要对号入座）
 
 其实原生APP发展到现在也算到了一个瓶颈，除了游戏，一般的功能型APP的模式几乎就那么几种
 而且对于小型创业公司来说，跨平台开发简直是，难得一逼，当你找来安卓工程师和ios工程师，你兜里的 `马尼` 也剩不下多少了。
 
 >其实，用写网站的语言是可以写APP的。
 
对于一个前端工程师，WebAPP开发起来，可以说是零门槛， `出道既辉煌，虐你没商量` 。

**但是** 为什么现在绝大多数APP还是原生写的呢？

最主要的原因，还是性能。当有一天WebAPP的性能发展到足够与原生APP媲美的时候，不用说别的，WebAPP跨平台开发这一项就能干掉原生APP。
这一天会到来么？肯定会，时间长短的问题。
（玩原生的不要喷我，我随便说说的）

不扯没用的，开发WebAPP，你有很多选择：`Ionic` `APICloud` `Dcloud` 等等等。
观望了许久之后，我选择了 `mui`-`Hbuilder`-`5+Runtime`————也就是`Dcloud`。

几个下午之后，写出了一些作品，也有一些感悟，但 `眼前有景道不得，崔颢题诗在上头` 。
看了 [小青年](http://zhaomenghuan.github.io/#!/blog/20160515) 的博文之后，还是自叹弗如。

下面大部分为转载（已被授权），又是一波干货来袭——————mui初级入门教程（一）— 菜鸟入手mui的学习路线
P.S. 陆续更新
<!--more-->

## **写在前面**

相信很多朋友初次接触到`dcloud`这边的产品，一般都是`hbuilder`和`mui`，所以很多朋友对于`dcloud`这边的产品链的认识也是各不相同。我相信对于很多新手来说，初次使用`dcloud`这边的产品的第一感觉一定是觉得这个东西很好却无从下手，然后被一些新的概念转得云里雾里，然后就开始吐槽官方文档，其实真的是文档不好吗？

稍微有点基础的开发者可能仔细去看看官方文档，然后就可以自己跟着文档或者demo做点小例子，然而很多人由于是业务临时需要才转到跨平台app开发的，很多可以说零基础，即使有文档也不定会看得懂，或者看了更晕，相信这部分开发者最期待的是有人手把手教最好，我见过很多开发者一上来一言不合就要例子，如果你让他去看`hello mui,hello h5+`这两个最精华的例子，他也许会觉得你在逗他。

其实这是因为我们很多时候把精力搞分散了，没有把力量集中起来去逐个突破，所以导致看起来感觉到处是肉，啃起来到处是骨头。哈哈，说了这么多，你可能觉得是废话，你也可能觉得说到你心理去了，如果你对`dcloud`这边的产品还是有点不明不白，那希望你耐心看下面的分析，也请你等待我后续的基础教程。


## **资源索引**

先把几个常用的地址丢出来，因为你如果不想看我后面的，你直接去看这些也可以！

### 新手值得收藏的地址

 * Dcloud官网：[http://dcloud.io/](http://dcloud.io/)
 * Dcloud问答社区：[http://ask.dcloud.net.cn/](http://ask.dcloud.net.cn/)
 * Dcloud文档汇总地址：[http://ask.dcloud.net.cn/docs/](http://ask.dcloud.net.cn/docs/)
 * Hello mui演示APP下载地址：
 ![Hello mui演示APP](https://raw.githubusercontent.com/jeasonstudio/images/749c8168af9dea6b6318b2672ceb5f123097950b/20160611/Hello%20muiAPP.png)
 * HTML5+ 演示APP下载地址：
 ![HTML5+ 演示APP](https://raw.githubusercontent.com/jeasonstudio/images/749c8168af9dea6b6318b2672ceb5f123097950b/20160611/HTML5%2B%20APP.png)
 * 官方入门文档:
   - [Dcloud 产品概述](http://ask.dcloud.net.cn/docs/)
   - [APP 入门开发](http://ask.dcloud.net.cn/docs/#http://ask.dcloud.net.cn/article/89)
   - [mui 产品](http://ask.dcloud.net.cn/docs/#http://ask.dcloud.net.cn/article/91)
   - [新手指南](http://dev.dcloud.net.cn/mui/getting-started/)
 * 案例汇总：[http://dcloud.io/case/](http://dcloud.io/case/)
 * GitHub 地址：[https://github.com/dcloudio/](https://github.com/dcloudio/)
 * 开源项目地址：[https://github.com/dcloudio/casecode](https://github.com/dcloudio/casecode)
 
## **官方分类文档**

 * html5+官网文档：[http://www.html5plus.org/doc/](http://www.html5plus.org/doc/)
 * mui ui组件文档：[http://dev.dcloud.net.cn/mui/ui](http://dev.dcloud.net.cn/mui/ui)
 * mui javascript文档：[http://dev.dcloud.net.cn/mui/event](http://dev.dcloud.net.cn/mui/event)
 * 5+ App开发Native.js入门指南：[http://ask.dcloud.net.cn/article/88](http://ask.dcloud.net.cn/article/88)
 * Native.js示例汇总：[http://ask.dcloud.net.cn/article/114](http://ask.dcloud.net.cn/article/114)
 * 流应用开发指南：[http://ask.dcloud.net.cn/article/406](http://ask.dcloud.net.cn/article/406)
 
## **其他学习资源**

 * [0Hich的网校视频](http://dcloud.apk00.com/)
 * [东翌学院视频](http://www.dongyixueyuan.com/)
 * [51CTO学院-张伟芝老师视频](http://edu.51cto.com/course/course_id-5086.html)
 * [猿团视频](http://edu.yuantuan.com/course/explore/DCloud?fliter%5Btype%5D=all&fliter%5Bprice%5D=all&fliter%5BcurrentLevelId%5D=all&orderBy=latest)
 * [E家课堂视频](http://www.ejiakt.com/album/show/231)
 * [网友YanRong的心得](http://ask.dcloud.net.cn/article/217)
 * [滴石App开发者的心得](http://uikoo9.com/book/chapterDetail/1)
 * [小青年博客](http://zhaomenghuan.github.io/)
 
## **学习路线**

当我列出上面的这些网址，我发现其实文档并不算少，但是新手为啥感觉还是很难呢？我们会发现一个问题，官方文档很分散，或许分散了导致开发者每次遇到问题查找文档的范围可能或许片面，其实也许他把所有的看完了就会找到答案，但是一般人恐怕没那么耐心吧，还有新手根本就没有一个清晰的思路，所以很难快速去找到自己需要的文档，所以我想官方文档需要统一化具体化。

而且把这些大致浏览一下会发现内容真多，光html5+里面的标准就那么多，一个个去认真学习完到猴年马月去了，mui组件也那么多，难道也要一个个学习？还有native.js、流应用等等，感觉太多东西了，是不是瞬间觉得头大了，哈哈，人总是有点偷懒的，如果有人帮我们写好现成的我们直接用那就好了，于是dcloud这块想了很多办法让开发者去开心开发，hbuilder丰富的语法提示、代码快捷键、真机调试、演示demo等等，mui提供了丰富的组件，如果熟悉这些，开发起来还是很快的。

前提是熟悉了以后才会爽，如果不熟会感觉什么，学的东西太多，比如熟悉hbuilder都要一段时间，然后熟悉html5+，native.js，页面布局和写逻辑功能，对于新手来说，门坎儿并不小，这也是为啥很多新手喜欢吐槽的原因。因为当开发者熟悉了基本流程，会发现dcloud这边相对其他平台来说更开放，个人可定制空间更大，正因为越发开放，那么可以应用的场景更加广泛，自然开发者问题更多，这也希望有能力的开发者能够去完善整个开发生态链。

这里给各位的建议是先熟悉html5+的常用api，比如webview，你只有对html5+里面的webview有所了解，才能理解为什么mui里面会去封装一些原生实现的组件如双webview的上拉刷新，tabbar多子页面底部导航等。mui里面的这些组件通过对html5+ webview的封装，极大的提升了app的性能。由于用hbuilder打包的app默认包含html5+ rumtime，所以当你使用hbuilder构建app项目时候，无论你是否引用mui文件，无需引用任何其他文件，你都可以调用html5+ api和native.js。也就是说即使你不用mui，只用html5+提供的api，然后自己书写html，css，js文件就可以打包生成一个app。

当然考虑到大部分人时间精力有限，为了让开发者有较快的开发速度，官方提供了mui框架，mui框架拥有丰富的组件，可以极大的提高开发效率。根据hello mui演示app提供的demo，开发者可以快速构建一个自己的app。

mui是基于html5+构建的框架，所以对于mui中提供的原生组件，其适用环境是app中的原生组件webview，并不能在浏览器中运行，如果想用mui构建浏览器上的手机站点，只能使用mui中基于h5的组件。对于原生实现的组件，mui都有对应的h5实现，所以开发者可以做合理的处理，在书写较少代码的情况下，实现多端发布。

流应用是dcloud这边很有创新的一个产品，流应用基于HTML5+技术，可达到原生应用的体验。同时基于DCloud专利的流式发行和更新技术，可以大幅压缩安装包并实现边下边用。让App可5秒内完成下载、启动。目前拥有6亿手机用户的360手机助手已经集成了DCloud的流应用引擎，可以发行流应用。建议对dcloud的产品有个大致了解后再实践这块的内容。

所以我给新手的学习路线是hbuilder = > html5+ = > mui = > 多端发布和流应用，当熟悉了这边的产品链以后开发起来会快很多，像hbuilder,html5+开始可以简单看看，了解基本的东西就可以。用mui的话至少得有基本的前端基础吧，再怎么样也得会基本的css布局和js基础吧，如果没有这些基础，先花点时间学一下基础或许更好。不要相信那种什么从零开始一周开发app的广告词，没有基础，也很难说做一个体验极好的app。

如果有原生开发经验的开发者一定会理解java在android中或者Objective-C在ios中的地位，做跨平台app开发，其实主要还是在于js功底，特别是原生js水平，所以如果js基础一般的开发者还是要不断加强学习，这里给的建议跟着hello mui里面的例子学，看官方人员是怎么写的，自己学着写，然后也可以在业余时间去研究一下基础。相信假以时日，你会发现你的js水平也会不断提高。
   

## **学习疑惑解答**

### html5+是什么？

html5+是DCloud提供的html5强化引擎，可以把HTML5 App打包为原生App，并且达到原生的功能和体验。说白了就是原本只能原生APP才能实现的功能，现在可以通过html5+这个强化引擎作为桥梁，你通过调用plus.*方法实现，也就是你可以通过书写js代码实现android和ios两套的原生功能。html5+封装了一些最常用的功能，并向W3C提交了作为标准的提案，具体的可以参考[html5+规范API](http://www.html5plus.org/doc/)。

### html5+和native.js有什么区别？

html5+作为一种通用标准，只封装了最常用的一些API，如果你有其他需求但是5+里面没有怎么办，这个时候如果你懂原生应用开发，你可以基于native.js语法规范进行个性化封装。Native.js for Android封装一条通过JS语法直接调用Native Java接口通道，通过plus.android可调用几乎所有的系统API。Native.js for iOS封装一条通过JS语法直接调用Native Objective-C接口通道，通过plus.ios可调用几乎所有的系统API。

### 5+ sdk是什么？

我们经常看到html5+(即html5plus)、5+ sdk,其实本质是一样的，不过这里的5+ sdk是针对离线打包开发和Hybrid开发模式，因为用hbuilder在线打包，html5+和native.js的底层会被自动打包到安装包里面，开发者无需引用什么即可调用相关API。只要当开发者想要离线打包及Hybrid开发模式或者深入了解html5+的引擎实现原理，才需要去了解一下5+ sdk，一般情况下我们只需要知道5+标准里面的基本用法就足够我们开发出一个APP。

### mui与html5+有什么关系？

mui是Dcloud官方推出的一个基于html5+标准的框架，同时拥有h5组件和原生组件，原生组件依赖于html5+运行环境，也就是原生app里面的webview组件（能加载显示网页，可以将其视为一个浏览器），所以mui里面的原生组件不能用于浏览器环境，可以通过mui里面的mui.os.plus进行判断，如果是plus环境会返回true，否则会返回undefined。开发者可以根据自己的需要进行代码适配，对于APP使用增强的原生组件，对于普通浏览器里面运行的页面使用h5组件。同时用户还可以使用mui.os.android、mui.os.ios及mui.os.wechat对平台进行检测，然后书写不同的逻辑代码。对于mui里面没有封装的原生组件，大家可以根据自己的需要基于html5+标准和native.js语法进行个性化定制。因此这里我们可以有一个基本影响就是我们开始可以直接上手mui，不过需要明白mui与其他UI框架的区别在于，mui拥有独有的原生组件，而且这个是依赖于html5+标准的，所以mui里面的很多组件实现方法甚至用户就是html5+里面的标准写法，对html5+标准有一定了解有助于我们理解mui的一些使用方法。

---

## **写在后面**

快考试周了，不多说，且行且珍惜。

放上来几个我自己刚写的APP，我还是个小白，不过，摸索中才能成长，希望有好的APP想法的童鞋多跟我交流
`想法总是要有的，万一我把它实现了呢`

![钢镚儿](https://raw.githubusercontent.com/jeasonstudio/images/749c8168af9dea6b6318b2672ceb5f123097950b/20160611/gangbenger.jpg)

![SayLoveMe](https://raw.githubusercontent.com/jeasonstudio/images/749c8168af9dea6b6318b2672ceb5f123097950b/20160611/SayLoveMe.jpg)

看到结尾的都是真爱。

