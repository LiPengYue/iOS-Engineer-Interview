[TOC]
# 岱宗夫如何？齐鲁青未了

## 说明

- 该仓库主要目的是为参加面试做准备
- 在复习中，对于面试中会遇到的包括iOS，算法，计网都进行了研究
- 对于iOS方面，比较深的感触应该就是研读了很多的源码，把以前很多只会使用的知识都了解了下底层原理，使用规范等等
- 以及对于一些之前只是当作简单的知识点死记硬背的地方，学着学着也发现了其中的原理，感觉对于iOS开发的有利新的理解
- 在之前的学习中，常常感慨没有一本好的教科书，没有真正意义上系统的iOS开发路线，总感觉自己学的半懂不懂，很多时候都停留在会用这个很基础的阶段
- 但现在看来，这些其实都算不上什么借口，真正阻碍我们的，只是你想不想学，愿不愿意学的深一点
- 与其感慨路难行，不如马上出发！

## 大二暑假

### 时间范围

- 2019.7.13 ～ 2019.8.16
- 其中7.21 ～ 8.16为实验室规定的统一的留校时间，前面一周是刚考完试自己的学习时间

### 目标

- 下一学期10月底左右参加面试，并在寒假参与日常实习
- 暑假将面试会考到的知识基本都涵盖到，开学那两个月进行复习

### iOS基础相关（必会，面试必问）

#### 语言和底层相关【重要： 面向对象的三大特性（关于OC）】：

1. ARC与MRC的区别&&RunTime&&RunLoop
  - ARC与MRC的区别
    - [ARC和MRC](https://www.jianshu.com/p/5eac83471b23)
  - RunTime讲述整个轮廓
    - weak底层实现
  - RunLoop要了解
    - [autoreleasePool](http://blog.leichunfeng.com/blog/2015/05/31/objective-c-autorelease-pool-implementation-principle/)
3. 属性关键字&&循环引用&&Category&&消息发送三次拯救
  - [深入理解Objective-C：Category](https://tech.meituan.com/2015/03/03/diveintocategory.html)
4. 探索block的原理
  - 要求能独立描述block的整个实现
  -  可参考《iOS高级编程》
5. KVC、KVO原理、单例、代理、iOS 存储
  - 每个人必须熟悉
6. 多线程编程 GCD、 NSOpearation（线程安全、死锁）网络请求的几种方式
  - 了解NSURLSession 、NSURLSession 和NSURLConnection区别、第三方框架AFN
#### UI相关：
- 响应者链
- 贝塞尔曲线、CALayer
- iOS native 与 js 交互(JSBrdige)

### 计算机基础相关（必会，面试必问）

- 数据结构
	- 链表的常见算法：例如 逆置
	- 二叉树的常见算法： 例如 三种遍历（递归和非递归）
	- 可参考：[博客](https://blog.csdn.net/qq_38499859/article/list/2?)
- 算法
  - [Leetcode](https://leetcode-cn.com) 面试官经常从这里面抽题问
  - 根据个人进度，暑假每人最少刷够10道
- 计算机网络
- 《图解HTTP》（可选）
	- 需要知道从点击一个URL到显示的整个过程，对这部分不了解的必须看

## 大二暑假总结

- 整个七月八月合起来一共写了15篇博客，基本上都是对iOS的深度解读，算是没有一片水文，都是呕心沥血之作
- 在暑假前有跟学长学姐交流过，当时真的只是对于RunTime，RunLoop有个很模糊的理解，大概就知道有个weak很难很难，RunLoop实现原理很复杂，就知道这些简单的概念，我就直接出发，开始源码解读之路
- 在暑假前，对于暑假留校我的理解大概是：很滑，很水，大二老油条了，带带大一，写写项目，总不能还得早八晚十吧！
- 结果这TM就是个天大的flag，整个暑假我基本上比大一要勤奋多了，完全不敢迟到，天天早上0洗漱冲到实验室，坐下LeetCode上刷一道题，过了半个小时才敢溜回去刷牙洗脸。。。
- 对我们的学习任务是到暑假前两个星期左右布置下来的，在这之前，我竟然一直在怕没什么好学的，感觉整个暑假会虚度，直到任务单发下来，发现自己基本没什么会的，才知道，虚度是不可能虚度的，榨干更有可能
- 我比较的好的一方面是在暑假前就有web组的同学提出要跟我合作写一个H5+Native混合开发的项目，所以一开始我不是很慌，觉得自己这么都有事做
- 我那时考虑的好像是两周之内写完这个项目。。。
- 任务下来以后我认真瞅了瞅，我尼玛，这怎么学得完，直接放弃回家的念头，决定干脆在学校呆着【暑假第一个星期实验室留校还没开始】
- 那一个星期实验室基本上就我一个人，每天坐在工位上，早上泡杯茶，开始看《iOS高级编程》，一直就看到太阳西沉，陪着我的只有左边的地狱咆哮
- 这一周把小白书的MRC，ARC部分全部看完，开始看RunTime源码，写了第一篇源码导读博客《基本结构体》
- 当时还没有买Apple pen，在笔记本上写了好多笔记，我印象最深的应该是引用计数的打印那块，老是出乎意料，就迫不及待地开始读源码了
- 读源码的时候有意思的事蛮多的，比如最早找到的源码全是OC 1.0时候的源代码，啃了半天，点进去宏定义发现这部分代码根本不生效。。。
- 暑假里iOS方面没有完成的就是Block和Category这两块，其实读源码也没有什么难的地方，就是画图，一点一点看流程
- 唯一让我很烦的应该是GCD那块，当时没有好好学，对于打印顺序一直整不明白

![D557741A084A76D09C895400585C9241](https://tva1.sinaimg.cn/large/006y8mN6ly1g90644wcwlj30to0m8aee.jpg)

# 造化钟神秀，阴阳割昏晓

- 大三了，大学生涯即将结束，对于我的面试也没多少时间啦，但是算法还没刷，项目还没完结，计网还没看
- 救命，救救孩子
- 这段时间把Block补完，之后花了两周左右一直在看算法网课，算是开开视野
- 同时把项目中的下载那一块实现了基本的功能，虽然不是很难，但是规划这样一个文件项目，让我学到了很多东西

# 荡胸生曾云，决眦入归鸟

- 离我规划的正式投简历时间大概就一个月不到了
- 这里我开始翻看之前的博客，看一些总结性的iOS网课，将Category这类之前没有好好准备的
- 这一部分还包括市面上我搜到的所有面试题
- 多线程
  - 幕布链接：https://mubu.com/doc/lenYY-w2Q0
  - 这一部分包括GCD，NSThread，NSOperation以及搜到的多线程面试题
  - 主要内容都来自不羁阁的博客，我觉得多线程看他的就OK
- 内存管理：
  - 幕布链接：https://mubu.com/doc/apZhNMVeZw
  - 这一部分主要来自自己的博客，都是小白书上关于ARC，MRC的部分
- RunTime：
  - 幕布链接：https://mubu.com/doc/8cd4n4LoBw
  - 这一部分都是自己过往博客提炼出来的知识点
  - Category那一块是边学边总结的
- 属性关键字：
  - 幕布链接：https://mubu.com/doc/yg8tZgFlK0
  - 这一部分强调了copy
- Block：
  - 幕布链接：https://mubu.com/doc/og_Yq8zpK0
  - 这一部分主要来源于自己的博客
  - block比较复杂，还是贴了一堆源码
- RunLoop：
  - 幕布链接：https://mubu.com/doc/tgsuA4Qto0
  - 主要部分来自于不羁阁的博客，迦蓝的博客补充了一下
- 事件传递：
  - 幕布链接：https://mubu.com/doc/daTBx-INBw
  - 主要部分来自于刘小壮的博客，壮哥威武
- 设计模式：
  - 幕布链接：https://mubu.com/doc/hx2K5yQE20
  - KVC不算设计模式，但是复习的时候发现很多人说KVO是基于KVC实现的，虽然我感觉关系不是很大，我也放进去了
  - 这一块算是我特别不知道学什么的一部分，很多地方没怎么仔细看过去
- MVC与MVVM：
  - 幕布链接：https://mubu.com/doc/ryHNiukoS0
  - 了解为主，了解为主

# 特别鸣谢

## 说明
- 在各个部分的参考文章里吧主要的参考文章都列出来了，但是对于GitHub上clone的资料没有提到，就放在这里统一鸣谢，感谢这些大大的精彩分享
## 名单
- [acBool / RuntimeSourceCode](https://github.com/acBool/RuntimeSourceCode)
- [DeveloperErenLiu / RuntimePDF](https://github.com/DeveloperErenLiu/RuntimePDF)
- [RuntimeAnalyze](https://github.com/DeveloperErenLiu/RuntimeAnalyze)