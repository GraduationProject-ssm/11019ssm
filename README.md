# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 11019ssm汽车在线销售系统

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Kp48e9EtU?p=65)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

汽车在线销售系统工作原理图如图4-1所示：

![](/md/blog.010.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。汽车在线销售系统的整体结构设计如图4-2所示。

![](/md/blog.011.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
概念模式它主要是建立在数据需求分析的基础上，它通常是用概念数据模型来表示各个数据之间的联系，并且对系统用户进行信息的处理和管理，同时建立起E-R图来表示具体的实体、属性和联系的关系。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，公司中的每个员工，家里中的每个家具。

本系统的E-R图如下图所示：

1、用户管理实体图如图4-3所示：

![](/md/blog.012.png)

图4-3用户管理实体图

2、车辆信息管理实体图如图4-4所示：

![](/md/blog.013.png)

图4-4车辆信息实体图

3、管理员信息管理实体图如图4-5所示：

![](/md/blog.014.png)

图4-5管理员信息管理实体图

### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表4-1：allusers表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|ID|int|11|PRIMARY KEY|
|username|varchar|50|DEFAULT NULL|
|pwd|varchar|50|DEFAULT NULL|
|cx|varchar|50|DEFAULT NULL|
表4-2：yonghu表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|zhanghao|varchar|50|DEFAULT NULL|
|mima|varchar|50|DEFAULT NULL|
|xingming|varchar|50|DEFAULT NULL|
|xingbie|varchar|50|DEFAULT NULL|
|chushengnianyue|varchar|50|DEFAULT NULL|
|lianxidianhua|varchar|50|DEFAULT NULL|
|dianziyouxiang|varchar|50|DEFAULT NULL|
|shenfenzhenghao|varchar|50|DEFAULT NULL|
|`	`shouhuodizhi|varchar|50|DEFAULT NULL|
|gerenzhaopian|varchar|50|DEFAULT NULL|
表4-3：cheliangxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|addtime|varchar|50|DEFAULT NULL|
|cheliangbianhao|varchar|50|DEFAULT NULL|
|cheliangmingcheng|varchar|50|DEFAULT NULL|
|cheliangleixing|varchar|50|DEFAULT NULL|
|qichetupian|varchar|50|DEFAULT NULL|
|cheliangyanse|varchar|50|DEFAULT NULL|
|huandangfangshi	|varchar|50|DEFAULT NULL|
|cheliangtianchuang|varchar|50|DEFAULT NULL|
|chezuo|varchar|50|DEFAULT NULL|
|qichepailiang|varchar|50|DEFAULT NULL|
|cheliangjiage|varchar|50|DEFAULT NULL|
|cheliangkucun|varchar|50|DEFAULT NULL|
|cheliangxiangqing|varchar|50|DEFAULT NULL|
|thumbsupnum|varchar|50|DEFAULT NULL|
表4-4：rukujilu表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|addtime|varchar|50|DEFAULT NULL|
|cheliangbianhao|varchar|50|DEFAULT NULL|
|cheliangmingcheng|varchar|50|DEFAULT NULL|
|cheliangpinpai|varchar|50|DEFAULT NULL|
|cheliangleixing|varchar|50|DEFAULT NULL|
|cheliangyanse|varchar|50|DEFAULT NULL|
|cheliangkucun|varchar|50|DEFAULT NULL|
|dengjiriqi|varchar|50|DEFAULT NULL|


# 5系统界面实现
## 5.1 前台功能模块
网站首页
## 网页首页汽车在线销售系统模块如下：首页、汽车信息、新闻资讯、留言反馈、我的收藏管理等功能图5-1
![](/md/blog.015.png)     
图5-1网页首页

网页前台车辆信息效果图如图5-2所示

![](/md/blog.016.png)

图5-2 车辆信息界面图
###  
## 5.2  管理员功能模块
`   `管理员输入个人的账号、密码登录系统，这时候系统的数据库就会在进行查找相关的信息，如果我们输入的账号、密码不正确，数据库就会提示出错误的信息提示，同时会提示管理员重新输入输入自己的账号、密码，直到账号密码输入成功后提示

成功登录成功的信息。网站管理员登录效果图如图5-3所示：

![](/md/blog.017.png)

图5-3管理员登录信息管理界面
### 5.2.3 用户信息管理 
管理员对用户信息管理编辑账号 密码姓名 性别 出生年月 联系电话 电子邮箱 身份证 收货地址 个人照片 进行添加、查看、修改以及删除等操作。程序效果图如下图5-4所示：

![](/md/blog.018.png)

图5-4用户信息管理 界面
### 5.2.4车辆信息管理
管理员对车辆信息管理编辑车辆编号 车辆名称 车辆品牌  车辆类型 汽车图片 车辆颜色  换挡方式 车辆天窗  车座 汽车排量 车辆价格 车辆库存 车辆详情 进行添加、删除、修改以及查看等操作。程序效果图如下图5-5所示：

![](/md/blog.019.png)

图5-5车辆信息管理界面
### 5.2.5出库记录管理
管理员对出库记录管理信息进行、删除、修改以及查看等操作。程序效果图如下图5-6示：

![](/md/blog.020.png)

图5-6出库记录管理界面
### 5.2.6入库记录管理
管理员对入库记录管理编辑车辆编号 车辆名称 车辆品牌  车辆类型 汽车颜色 进行删除、修改以及查看等操作。程序效果图如下图5-7所示：

![](/md/blog.021.png)

图5-7入库记录管理界面
### 5.2.7 车辆购买管理
管理员对车辆购买管理编辑车辆编号 车辆名称 车辆品牌  车辆类型 汽车颜色信息进行删除、修改以及查看等操作。程序效果图如下图5-8所示：

![](/md/blog.022.png)

图5-8车辆购买管理界面
### 5.2.8运输收费管理
管理员对运输收费管理进行删除、修改以及查看等操作。程序效果图如下图5-9所示：

![](/md/blog.023.png)

图5-9运输收费管理界面


### 5.2.9留言板管理
管理员对留言板管理进行删除、回复以及查看等操作。程序效果图如下图5-10所示：

![](/md/blog.024.png)

![](/md/blog.025.png)

图5-10留言板管理管理界面

### 5.2.10系统管理
管管理员通过系统管理页面查看轮播图/新闻资讯等进行上传图片进行添加、删除、修改以及查看并对整个系统进行维护等操作，程序效果图如下图5-11所示：

![](/md/blog.026.png)

图5-11系统管理理界面界面





## 5.3  用户前台功能模块
### 5.3.1 登录
用户在注册完个人信息后会跳转到登录界面上，输入注册的登录账号及密码后才可登录。程序效果图如下图5-12所示：

![](/md/blog.027.png)

![](/md/blog.028.png)

图5-12登录界面图
### 5.3.2 个人中心
个人中心：在个人资料管理页面通过查看账号 密码姓名 性别 出生年月 联系电话 电子邮箱 身份证 收货地址 个人照片 可进行查看进行修改、删除等 。程序成效图如下图5-13所示:



![](/md/blog.029.png)
### 图5-13个人中心界面

### 5.3.3 车辆购买
用户可以车辆购买进行查看、支付信息等操作。程序效果图如下图5-14所示：

![](/md/blog.030.png)

![](/md/blog.031.png)

图5-14车辆购买界面
### 5.3.4 运输收费管理
用户查看运输收费管理详情并可以展开查看、支付等操作。程序效果图如下图5-15所示：

![](/md/blog.032.png)

图5-15运输收费详情界面
### 5.3.5 订单状态管理
用户查看订单状态管理详情并可以查看状态等操作。程序效果图如下图5-16所示：

![](/md/blog.033.png)

图5-16订单状态管理界面
### 5.3.6 我的收藏管理
用户查看我的收藏管理详情在前台看到有喜欢的车辆并可以展开收藏等操作。程序效果图如下图5-17所示：

![](/md/blog.034.png)

图5-17我的收藏管理详情界面












