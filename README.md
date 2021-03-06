# 漫画书
#####1.平台：Android客户端（后期完善IOS端）
#####2.开发框架：React Native     react-redux     react-thunk
#####3.开发工具：Vs Code 1.8
###1.项目架构
#####app
#####actions 用户行为
#####reducer 对用户行为进行分发，更新状态
#####store   整合全部reducer
#####container  业务模块
#####components UI组件
#####utils      工具文件
#####images     图片
#####constan    常量
#####style      样式
#####api        网络URL
#####widget     自定义组件
#####root.js    App根文件
#####app.js     App入口
#####index.ios.js
#####index.android.js
#####项目采用React-Native   react-redux   react-thunk框架开发，目前由于没有mac设备，只完成兼容Android环境，代码模块化实现，组件封装实现代码复用。

###2.App模块

 分为首页、发现、精选、我四大版块，以下是功能列表：

    1.使用ViewPager跟ListView展示图文列表。
    2.推荐精彩漫画列表。
    3.精选内容，分类展示，增加滑动Tab，增加用户体验。
    4.自定义扩展ListView，实现上拉加载更多数据，下拉刷新数据。
    5.添加缓存功能，增强用户体验。

项目用到的接口来自聚合数据。
###3.整体设计

#####使用官方的Navigator管理全局路由，可自由配置Scene的出场动画，处理Android端的后退键事件
#####使用FlexBox和jsx语法进行布局，并封装了一系列通用的组件，比如TopBar 、带上下拉功能的ListView等，便于全局复用
#####导入第三方库react-native-wechat实现微信分享
#####使用InteractionManager，阻止ListView的头部和尾部频繁刷新，优化渲染性能。
#####在深刻理解的前提下引入redux相关功能，包括redux/react-redux/redux-thunk/，设计与漫画列表和详情相关的全局state结构，使用redux管理相关的组件

###4. 第三方库 
#####依赖方式，cd到项目根目录，执行： npm install [插件名称] -save
#####(1)redux: ^3.6.0
#####(2)react-redux: ^5.0.2
#####(3)react-thunk: ^1.0.0
#####(4)redux-thunk: ^2.1.0
#####(5)react-native-blur: ^2.0.0
#####(6)react-native-viewpager
#####(7)react-native-vector-icons: ^4.0.0
#####(8)react-native-scrollable-tab-view: ^0.7.0
#####(9)react-native-lightbox: ^0.6.0
#####(10)react-native-simple-store: ^1.1.0
###5.运行截图
<img width="300" height="500" src="http://img.blog.csdn.net/20170210111205969"/>
<img width="300" height="500" src="http://img.blog.csdn.net/20170210110535276"/>
<img width="300" height="500" src="http://img.blog.csdn.net/20170210111244016"/>
<img width="300" height="500" src="http://img.blog.csdn.net/20170210111336377"/>
<img width="300" height="500" src="http://img.blog.csdn.net/20170210111512390"/>
<img width="300" height="500" src="http://img.blog.csdn.net/20170210111557077"/>
<img width="300" height="500" src="http://img.blog.csdn.net/20170210110405349"/>
