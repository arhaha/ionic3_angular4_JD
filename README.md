## ionic3_angular4_JD ##

最近在逛淘宝的时候，居然看到有人在卖我的源码，标价十元，已经卖出几份，为买了的人心疼，为了打击二道贩子

##### 现代码所用采用GPL协议开源！！！！！禁止用作商业用途！！ ####
##### 现代码所用采用GPL协议开源！！！！！禁止用作商业用途！！ ####
##### 现代码所用采用GPL协议开源！！！！！禁止用作商业用途！！ ####

重要的事情说三遍，此项目只能用于学习和交流，有什么问题大家可以提ISSUE，我自己也在在尝试把AG4作为前端主要框架使用，都是菜鸟大家可以多交流,哈哈，没办法我是谷歌粉

有关于wiki，我会写一写教程，比如：

[为什么都是UI，没有什么参考性，我加了一个简单版的购物车](https://github.com/dicallc/ionic3_angular4_JD/wiki/%E4%B8%BA%E4%BB%80%E4%B9%88%E9%83%BD%E6%98%AFUI%EF%BC%8C%E6%B2%A1%E6%9C%89%E4%BB%80%E4%B9%88%E5%8F%82%E8%80%83%E6%80%A7%EF%BC%8C%E6%88%91%E5%8A%A0%E4%BA%86%E4%B8%80%E4%B8%AA%E7%AE%80%E5%8D%95%E7%89%88%E7%9A%84%E8%B4%AD%E7%89%A9%E8%BD%A6)


[ionic快速集成极光推送](https://github.com/dicallc/ionic3_angular4_JD/wiki/ionic%E5%BF%AB%E9%80%9F%E9%9B%86%E6%88%90%E6%9E%81%E5%85%89%E6%8E%A8%E9%80%81)

关于集成极光推送，代码中已经提交，需要去分支拉取代码

代码运行需要依赖极光的插件，才能运行
<pre>
    cordova plugin add jpush-phonegap-plugin --variable APP_KEY=your_jpush_appkey
</pre>

不懂得可以看上文的教程

### 使用 ###



##### 1.cnpm install或者使用npm install

##### 2.ionic serve  ####


##### 3有需要使用android/ios平台 ####


       ionic platform add ios/android

##### 4运行android/ios平台####
	ionic run android/ios


##### 5.预览界面 ####

----------

<img src="https://raw.githubusercontent.com/dicallc/ionic3_angular4_JD/master/gif/GIF.gif"  alt="上海鲜花港 - 郁金香" />



#### 6.可预览android版本apk

[点击下载apk](https://github.com/dicallc/ionic3_angular4_JD/raw/master/gif/android-release.apk)

#### 7.源码查看

[点击打开代码地址](https://github.com/dicallc/ionic3_angular4_JD)

----------
### 再次记录从NG1-4一下坑吧 ###

##### 1.scss的图片地址应该怎么写 ####

    background-image:url('../assets/img/sprites.png');
##### 2.懒加载 ####
懒加载问题，我看到ionic有组件支持，但是不是很完善，可以使用下面的库

[点击打开](https://github.com/tjoskar/ng-lazyload-image)

##### 3.请求网络 ####
这个是最纠结的，第一个ES6，rxjs不熟悉，看到了很多例子，都不是很懂，其中使用箭头函数还遇到一些坑
有一个简单的例子 [点击打开](https://www.djamware.com/post/58e657b680aca764ec903c2d/ionic-3-and-angular-4-mobile-app-example)

当然我在项目中用到了代码：**GoodsService.ts** 使用：**good-lists-page.ts**

##### 4.全局常量 ####

全局常量的编写是有意义的比如图片地址，URL等

<code>
<pre>
export const APP_SERVE_URL = 'http://88.128.18.193:8080/';

export const FILE_SERVE_URL = 'http://88.128.18.144:3333/';

 export const APP_SERVE_URL = 'http://localhost:8100';

export const FILE_SERVE_URL = 'http://localhost:8100/kit_file_server';
</pre>
</code>

#### 更多详细的看下面的思维导图吧，是自己做的笔记 更详细内容在gif文件中的思维导图 ####

<img src="https://raw.githubusercontent.com/dicallc/ionic3_angular4_JD/master/gif/daotu.png"  alt="上海鲜花港 - 郁金香" />

### 结语： ###
1.耗时两周自学angular4和ionic3，其实很多东西不一样了，还好有SS，自从学了前端，一直在墙外看资料，看了很多人记录的帖子，觉得应该回报一下开源了。


第三方js：
使用typings 添加**swipe**r(幻灯片)，**ng-lazyload-image**(懒加载)，**jquery**(快捷开发)

<br>

 最后，如果这个项目能帮到你，动动你的鼠标点一下start呗 


### 更新日志： ###

----------


**5/8/2017 12:24:10 AM**

> 完成登录界面
<br>
<br>

**5/9/2017 2:24:55 PM**

完成发现界面

> 顶部导航栏没有发现好的实现方式，目前只是可以滑动，点击后的效果不明显


<br>
<b>5/9/2017 5:25:19 PM  </b>

修改发现界面，模范辣品的分类界面

<br>


<img src="https://raw.githubusercontent.com/dicallc/ionic3_angular4_JD/master/gif/20170509172835.png"  alt="上海鲜花港 - 郁金香" />

 

<b>5/10/2017 12:21:58 PM  </b>

1.使用官方组件，cards，toobar，完成购物车界面，高仿京东

小结：总体全部使用ios样式，变化挺大的，估计下一步就考虑适配，和性能问题了，一次编译时间事件挺久的


<br>
<img src="https://raw.githubusercontent.com/dicallc/ionic3_angular4_JD/master/gif/image.png"  alt="上海鲜花港 - 郁金香" />


<b>5/11/2017 12:24:00 PM  </b>

1.分模块加载页面，使用--prod，检测代码，优化以后代码

2.优化后的apk可直接秒进入，不需要等待白屏

3.微调我界面的ui

4.添加key 可以直接打prod模式的release

    ionic build android --release --prod
 

<b>5/15/2017 5:18:38 PM   </b>

1.重新使用ionic的grid布局，解决css样式兼容性问题,意外的发现兼容性存在很大的问题

**如对于flex布局**


- android:UC的内核就不兼容
- ios:9.3系统+


[查询css样式兼容情况](http://caniuse.com/#feat=flexbox)

同时找到一个第三方css，可在不同内核实现flex布局

[flex.css](https://github.com/lzxb/flex.css)

待以后尝试一下了
