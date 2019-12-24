# API_ML_AI智能口红试色购物app 



发布日期|2019年12月11日
--------------|:-----------|
文件名称|智能美妆购物app（以口红为主）|
进度|进行中
发布人|谢颖
项目迭代|3_1

---
## 价值主张设计
### 一、背景
经调查显示，现如今有许多美颜相机能换妆添加滤镜甚至变脸的效果，假若能有一款产品可以将现有的美妆产品购物app的与美颜相机相结合，用户挑选感兴趣的商品，打开摄像头呈现美妆产品在脸上的效果，用户再选择需不需要这款商品进行购买。还有一些明星或者网红的仿妆能通过上传该明星或网红的化妆照片，推荐出画该妆容的美妆产品，并附上教程，用户可以通过美颜相机呈现在脸上的效果，选择性购买商品。

PRD1.加值宣言 3%
### （一）加值宣言
本产品旨在通过调用腾讯云中的人脸识别、人脸融合、图像分析等api技术实现美妆产品的试用及购买的功能，用户可以挑选感兴趣的美妆产品，线上就能实现试用效果，并给用户推荐挑选出更合适的商品。用户也能通过上传感兴趣的妆容图，找寻可画出此妆容的美妆产品。

PRD2.核心价值 3%

Question|Outcome
------------------------------------------------------------------|:-----------------
提供腾讯云ai技术中的人脸识别中的五官定位技术识别用户拍摄或上传的人脸照片|定位好用户的五官位置并分析其五官特点
使用人脸融合技术，通过快速精准地定位人脸关键点，将用户上传的照片与特定形象进行面部层面融合，使生成的图片同时具备用户与特定形象的外貌特征|帮助用户实现美妆试色试妆的效果帮助用户融合同款明星妆容的妆效
使用推荐系统和图像分析技术推荐出相关的美妆产品|用户可上传图片识别照片内的美妆产品，并给出产品的品类、使用人群、肤色等，可以进行产品聚类、相似商品推荐，实现个性化广告展示，提高购买转化。


优先级：基于美颜相机的部分功能，再调用腾讯云ai中的人脸识别和人脸融合技术，将美妆产品的美妆效果呈现在用户脸上。

次优先级：基于腾讯云中的，人脸识别和图像分析技术，检测出用户上传照片中的妆容效果中使用的美妆产品。
PRD3.核心价值与用户痛点 3%
#### 核心价值与用户痛点
核心价值|用户痛点
------------------|:-------
能在选取美妆产品时，将其产品使用效果可视化到摄像屏幕上，并可以检测到用户五官，呈现在用户脸上|用户在挑选美妆商品时并不知道上脸的效果如何
可以通过上传照片获得照片中的妆效及相关产品|用户在想寻找相似妆容的美妆产品却不知从何寻找，且想要同款妆效的产品
通过上传或搜索相关产品的内容或照片，显示出该产品的细节、颜色、使用手法等，以及相似产品的相似度，各类博主对该产品的测评分析|美妆产品种类太多，且不知道其中的区别
#### PRD4.人工智能概率性与用户痛点 3%

**用户痛点**
1. 用户对



**人工智能概率性**
- 人脸识别：腾讯云AI中的人脸识别api，人脸检测定位，可检测图片中的人脸并标记出人脸坐标，支持同时识别多张人脸。五官定位技术可以精准定位五官的位置，实现人脸美颜美妆、人脸变形、人脸漫画、人脸换脸、人脸贴纸等。基于人脸检测功能，可识别用户如年龄、性别、颜值等属性特征，对顾客画像自动分类，结合客户消费记录等信息，提供更精准的客群分层流量分析；同时结合产品促销信息，根据不同客群的属性，提供更生动的互动营销体验，提升顾客满意度，促进购物消费转化
- 人脸融合api：在美颜相机中，通过让用户上传两张人脸图片，实现对目标人脸进行美颜的目的，增加美颜功能的种类，提升用户体验。通过快速精准地定位人脸关键点，将用户上传的照片与特定形象进行面部层面融合，使生成的图片同时具备用户与特定形象的外貌特征
- 图像分析技术：可以识别出图片中的多个商品，并给出商品的品类、坐标，可以进行商品聚类、相似商品推荐，实现个性化广告展示，提高购买转化。

#### PRD5.需求列表与人工智能API加值 3%
需求列表：使用人工智能的加值是否反映到需求列表（核心功能的排序上）且PRD列出明显有可行及可用的API

  #|用户案例|重要性|技术
---|:------:|:-----|:-------
1|用户正在网上某购物平台挑选口红，但很苦恼不知道试在自己嘴上是什么效果|极其重要|人脸识别api和人脸融合api
2|用户在网上看到某明星的妆容很好看，想知道其同款美妆产品、美妆教程及上脸效果|重要|人脸融合api和图像分析技术

---

## 原型 20%
#### 原型1.交互及界面设计 5%
交互及界面设计：在PRD文件中是否有说明且原型是否有做到：交互及界面设计的某个核心交互环节使用了人工智能的加值


#### 原型2.信息设计 5%
信息设计：在PRD文件中是否有说明且原型是否有做到：信息设计的某个核心信息或设计使用了人工智能的加值

#### 原型3.原型文档 5%
原型文档：多少程度上有提供MVP可交互的原型文档，供它人在Github上下载使用

#### 原型4.口头操作说明 5%
口头操作说明：多少程度上在2-3分钟时间限制内，对听众留下了「的确这是个可行丶可用的人工智能加值产品」的印象

### API 产品使用关键AI或机器学习之API的输出入展示 15%
#### API1.使用水平 5%
使用水平：在PRD文件中是否有说明且展示，核心功能所应用的API之输入及输出


#### API2.使用比较分析 5%
使用比较分析：在PRD文件中是否有说明且提供连结证据，所使用的API是查找过最适用的（主要竞争者无或比较次），如考量其成熟度丶性价比丶等等

#### API3.使用后风险报告 5%
使用后风险报告：在PRD文件中是否有说明且提供连结证据，所使用的API类别的现在及未来发展性，如API市场竞争程度丶输入输出限制丶定价丶及可替代的程序库（改用自己开发的代码及数据库而不用API）等等

#### API4.加分项 3%
使用复杂度：用了2个以上机器学习与人工智能的API之输入及输出
