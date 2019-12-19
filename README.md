发布日期|2019/12/16
  ----  | ----    
Epic|博物馆地图服务小助手
文件现状	|完成
文件主人|杨亦昊
领头设计者|杨亦昊
领头开发者|杨亦昊
领头测试者|杨亦昊

# 第一部分：需求概述
***********
## 1.背景概述
* 现有国内大多数的博物馆仍然在使用纸质的博物馆导览地图，游客一般只能查看地图、看提示牌或者询问工作人员查看周边的服务设施（场馆、纪念品店、厕所等）寻找的过程繁琐复杂。

* 现有的博物馆都有残障人士相关的服务设施如残疾人厕所、残疾人通道，大多数的服务设置在博物馆较隐蔽的地方。考虑残障人士身体原因运动不便，还是比较难获得相关的服务。

## 2.产品介绍--价值宣言
用户打开博物馆地图助手微信小程序，小程序将获得游客目前的定位信息，系统会基于高德地理围栏api，返回游客目前的位置的周边服务设置的位置信息并提供简单的导航。帮助用户更加快速、方便地找到服务设施或游览的场馆。

## 3. 核心价值--功能优先级
* 最小可行性分析：着眼于游客的基本，解决游客寻找服务设施难的问题，便利游客游览。

 用户|功能|重要程度
  ----  | ----  |  ----  
普通游客|提供周边服务的位置信息|重要
残障游客|提供残障服务设施的位置信息|重要
全部游客|提供游览场馆的文字和语音介绍|次重要
## 4.用户痛点--使用场景
用户痛点：
* 博物馆的场馆、服务设施众多，游客想要找到自己想要的相关服务比较困难。      
* 残障游客行动不便，残障服务设施一般在博物馆较隐蔽的地方，寻找起来比较困难。

用户|使用场景|用户需求
  ----  | ----  |  ----  
普通游客  | 博物馆内部|    找到服务设施（厕所、礼品店、食品店）
残障游客 | 博物馆内部 |  找到残障服务设施  （轮椅出租、残障人通道）
全部游客| 博物馆内部 |  想要获得场馆的介绍信息  
## 5.API使用
高德地理围栏服务是一类HTTP接口，提供在服务端，增删改查地理围栏的功能，同时支持对于设备与围栏关系进行监控。高德地理围栏服务适用于需要针对特定区域，监控用户位置与区域关系的场景中，判断用户是否已经在对应的地理围栏区域内。
* 输入：游客当前位置
* 输出：返回周边服务信息
# 第二部分：产品原型设计
*********
[产品原型](http://baiyingv.gitee.io/api-museum-html)

## 1.产品架构图
![产品架构图](https://upload-images.jianshu.io/upload_images/9455351-e06450dd859d8619.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 2.使用流程图
![流程图A](https://upload-images.jianshu.io/upload_images/9455351-5001bb96c7de742a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![流程图B](https://upload-images.jianshu.io/upload_images/9455351-b68d5d42adbd09f6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![流程图C](https://upload-images.jianshu.io/upload_images/9455351-4c990cafb6425b11.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
## 3.产品原型
![主页](https://upload-images.jianshu.io/upload_images/9455351-709c3ee7cf749bc0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![我的周边](https://upload-images.jianshu.io/upload_images/9455351-daeb83d9786b0111.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![展览展馆A](https://upload-images.jianshu.io/upload_images/9455351-b148294fbd6fd129.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![展览展馆B](https://upload-images.jianshu.io/upload_images/9455351-40b9418686a41361.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![残障服务](https://upload-images.jianshu.io/upload_images/9455351-5420bdbf6ab29ac4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


