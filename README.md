# 截图自动拼接小工具 

## 源起

经常会有这样的需求：

需要将微信里面和某些人的聊天记录转发给其他人，然而聊天记录过长，需要一页页截图发送，接收者收到这种消息往往有点抓狂，毕竟要反复确认每张图之间的上下文关系。所以，更好的做法应该是在本地将这些截图评完拼接再发送。

需要将某篇长文分享给其他人，但是当前 App 的分享功能非常难用，而且经常会强制接收者安装当前 App (比如某秘) 才能继续浏览文章。又或者是仅想分享文章到票圈而不让人知道出处。

这些需求总让人想要把当前的截图素材先做拼接再发送。而在我做这个 DEMO 的时候，AppStore 只有一款做自动拼接的免费 App，但不付费就限制保存次数，蛋疼。所以作为程序员还是自己撸一个用吧。于是就有了这么一个 DEMO。


## 上架

2015 年做完这个 App 后编译到自己 iPhone 用就没再管它。最近老婆大人想用，天真地问我：“为啥你这个东西不能上 AppStore？”。解释一通后，老婆大人就默默给我买了一年期的苹果开发者账号，说：“卖 6 块，收入归我”。（我去，做了 5 年家养 iOS 开发工程师后，要开始做独立开发者了么？）

=。= 强烈怀疑这货能不能收回成本。

## UI

作为一个年迈的程序员，完成这种 App 功能不过一两个晚上的事情，但是最大的痛苦是为了要上线，画 icon，准备资源，设计还过得去的界面。

App 名是 Centaur，因为它也是拼接出来的啊。（好冷

Icon 的意思是将 3 块图进行叠加。当然也[有人](https://github.com/imoldman)理解成 “人到三十”。(年迈的程序员

## 原理

有兴趣的同学可以参考这篇文章： [记一个截图拼接的小工具](http://xiangwangfeng.com/2015/11/30/%E8%AE%B0%E4%B8%80%E4%B8%AA%E6%88%AA%E5%9B%BE%E6%8B%BC%E6%8E%A5%E7%9A%84%E5%B0%8F%E5%B7%A5%E5%85%B7/)

原理较为简单，当然为了在实际使用中得到更好的效果也做了不少的改良，详细可以参考代码。

## 使用方法

参考如下[视频](https://nos.netease.com/yx-web/c44174085943f8362ff95efef4e8ec46) 

## 已知问题列表

### 下载后编译失败，提示缺少库

请使用 workspace 打开工程

### 某些截图无法拼接

对于截图中有动图，背景贴图的情况并无法 100% 有效

### 3x 支持

因为原理问题，对 3x 支持并不好......恶魔魔买面膜
