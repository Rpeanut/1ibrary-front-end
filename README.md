# 一图：高校图书馆合作伙伴

* 产品主页：[https://1ibrary.github.io](https://1ibrary.github.io)

* Apple Store 下载地址：[https://itunes.apple.com/us/app/%E4%B8%80%E5%9B%BE/id1230892748?l=zh&ls=1&mt=8](https://itunes.apple.com/us/app/%E4%B8%80%E5%9B%BE/id1230892748?l=zh&ls=1&mt=8)

* 团队 GitHub 地址：[https://github.com/1ibrary](https://github.com/1ibrary)

* 前端 GitHub 地址：[https://github.com/1ibrary/1ibrary-front-end](https://github.com/1ibrary/1ibrary-front-end)

* 后端 GitHub 地址：[https://github.com/1ibrary/1ibrary-back-end](https://github.com/1ibrary/1ibrary-back-end)


## Screenshot

![](http://airing.ursb.me/image/1ibrary/1ibrary-1.jpeg-h600.jpg)

![](http://airing.ursb.me/image/1ibrary/1ibrary-2.jpeg-h600.jpg)

![](http://airing.ursb.me/image/1ibrary/1ibrary-3.jpeg-h600.jpg)

![](http://airing.ursb.me/image/1ibrary/1ibrary-4.jpeg-h600.jpg)

持续更新中，欢迎Star~ 欢迎下载~

---

## 1ibrary-front-end
> 一图app前端代码
## 时间轴

### 17.04.08
创建项目，编写NavigationBar组件,ShareNav组件。
编写网络请求工具库HttpUtils.js

by miemie

###  17.04.09
- 编写底部标签BottomTabs组件     
- 编写带有搜索栏的导航SearchNav组件    
- 编写首页的主体部分，即书目列表的ListView实现
- todo: 网络请求部分的代码还没有写（下拉刷新的实现）。       
接下来需要解决的分别是
- 搜索提示页
- 搜索结果页。

by miemie
  
### 17.04.10
- 完成搜索历史&推荐页
- 熟悉本地存储技术点AsyncStorage    

待做:    
- 搜索结果页

by miemie

### 17.04.11
- 完成搜索提示页
- 完成搜索结果页除ScrollableBar之外的部分
待做:    
- 搜索结果页
- 抽象出BookList组件，将BookItem设置为自定义    
后续思路:     
- 在每个BookItem上设定navigator组件，实现BookItem和Book详情页面的跳转

by miemie

### 17.04.12
> 今天一图这块啥也没干，晚上收到了新的设计稿，变漂亮了，大概想了一下构建，思路上没有很大的出入。
> 明天开始动工！^_^ 加油！💪

by miemie

### 17.04.13
- 对之前做的四个页面进行了新设计稿的改版
- 明天要做的图书详情页思路：先分页面把每个页面实现，然后用navigator实现页面间跳转
- 出现的问题:ScrollableTabView组件不够灵活，暂时放弃自定义，后期如果有时间再补救

by miemie

### 17.04.14
- 改版顶部导航样式
- 完成图书详情页的基本布局

by miemie

### 17.04.15
- 完成首页部分的所有单个页面的布局和事件的编写
- 利用navigator实现页面之间的跳转

by miemie

### 17.04.16
- 完成书单的增加和删除部分
- bug: 书单这部分本来打算使用ListView这个组件，但当data改变的时候,ListView并没有变化，不得已最后使用了ScrollView然后map，这个以后需要留意，现在暂时没搞明白怎么回事

by miemie

### 17.04.17
>可以说是非常拼的一天了。。。。     

- 剩下登录页的两个页面没写
- 剩下个人页面的setting页和aboutus页没写

> 连写带改连续弄了8h。。。。。眼睛可以说是非常痛了。。。。😂
> 现在去躺尸。。。。。。

- 大boss: 网络层请求部分的代码 最后写
- 大boss: 排除所有的warning 网络层之前做 用chrome dev调试定位

by miemie

### 17.04.20
- 完成所有页面布局
- 明天测试网络层

by miemie

### 17.04.23
- 网络层局部测试成功
待做:    
- 所有网络层请求代码
- listview上拉刷新使用refreshcontrol来做，下拉加载参考[这篇回答](https://segmentfault.com/q/1010000004101829)
- 首页要做缓存 一开始先显示缓存 然后加载成功再刷新 书单在网络请求结束之后也要本地缓存
- 细节部分怎么完善？用户提示怎么做，用户不存在这些，统统暂时alert
- warning边做边排了一部分，集中排除要在最后
- 真机调试

by miemie

### 17.04.24
- 图书列表页面网络请求完成 图片无法加载
- 网络请求层代码与后端同步

by miemie

### 17.04.25
- 完善一些交互的细节
- 待做:
- 所有后端参数在前端都用props传递
- 同步后端api
- 交互排bug（为什么书单列表里面的书删完一个会影响下一个？？？？？）
- 楼上这个问题很烦，2h过去了
- 好气啊！！！！！！！

by miemie

### 17.04.26
## 除了书单列表里的删除效果很丑以外，基本完结了
ps 现在已经不丑了

by miemie

### 17.04.27
- bug: 启动页加载不出来 完全卡死
- 关于我们页面要新增webview 不过很明显现在进不去了
- webview这个比较简单 等启动页弄完之后参考[文章1](http://blog.csdn.net/codetomylaw/article/details/52490378)和[文章2](http://blog.csdn.net/wxs0124/article/details/50722135)即可     

下午四点更新:    
> 初稿完结

by miemie

### 17.04.29
- iphone 6s 点击问题修复
- 待做：
- 设置页面的按钮应该不滑动按钮也能动 像微信一样
- 完成按钮太小了

晚上update:   
以上问题全部解决

by miemie

### 17.04.30

- 添加了logo
- 修改了display name
- 修改了版本号
- 添加了LICENSE
- 尝试修改splash，尝试失败 _(:з」∠)_

提交 v1.0.2 审核

by Airing

### 17.05.01
今天点进去看小熊补充的内容。    
license添加进去了，不过关于我们里面版本号好像米有改？？？😂

by miemie

### 17.05.02
- 尝试修复滑动书单不灵敏的问题
- 修复删除后从书单进入列表页面时不及时刷新的bug

下午更新：    
震惊！！！之前一直以为无解的页面组件残留问题竟然被垂死梦中惊坐起的咩咩解决了哈哈哈哈哈哈哈！！    
然后修复了图书详情页面信息显示不完全的问题。     
^_^上课去。。。。。。    

by miemie

### 17.06.21
- 清行李回家的21号 开始重构一图

by miemie

### 17.06.26
- 新建common文件夹 编写styles.js 
- 待做： 更改未重构代码中的响应式高度和宽度的处理方式

by miemie

### 17.07.10
- 添加styles文件（内含设备长宽 响应式长宽获取函数）
- 添加Urls文件 聚合所有的url前缀和路径
- 复用楼上文件里的东西
- 修改文件名

by miemie

