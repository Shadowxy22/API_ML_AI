# API_ML_AI智能口红试色购物app 



发布日期|2019年12月11日
--------------|:-----------|
文件名称|智能美妆购物app（以口红为主）|
进度|进行中
发布人|谢颖
项目迭代|3_2

---
## 价值主张设计
### 一、背景
经调查显示，现如今有许多美颜相机能换妆添加滤镜甚至变脸的效果，假若能有一款产品可以将现有的美妆产品购物app的与美颜相机相结合，用户挑选感兴趣的商品，打开摄像头呈现美妆产品在脸上的效果，用户再选择需不需要这款商品进行购买。还有一些明星或者网红的仿妆能通过上传该明星或网红的化妆照片，推荐出画该妆容的美妆产品，并附上教程，用户可以通过美颜相机呈现在脸上的效果，选择性购买商品。

PRD1.加值宣言 3%
### （一）加值宣言
本产品旨在通过调用腾讯云中的人脸识别、人脸融合、人脸试妆、图像分析等api技术实现美妆产品的试用及购买的功能，用户可以挑选感兴趣的美妆产品，线上就能实现试用效果，并给用户推荐挑选出更合适的商品。用户也能通过上传感兴趣的妆容图，找寻可画出此妆容的美妆产品。

PRD2.核心价值 3%

Question|Outcome
------------------------------------------------------------------|:-----------------
提供腾讯云ai技术中的人脸识别中的五官定位技术识别用户拍摄或上传的人脸照片|定位好用户的五官位置并分析其五官特点
使用人脸试妆、人脸融合技术，通过快速精准地定位人脸关键点，将用户上传的照片与特定形象进行面部层面融合，使生成的图片同时具备用户与特定形象的外貌特征|帮助用户实现美妆试色试妆的效果帮助用户融合同款明星妆容的妆效
使用推荐系统和图像分析技术推荐出相关的美妆产品|用户可上传图片识别照片内的美妆产品，并给出产品的品类、使用人群、肤色等，可以进行产品聚类、相似商品推荐，实现个性化广告展示，提高购买转化。


优先级：基于美颜相机的部分功能，再调用腾讯云ai中的人脸识别和人脸试妆。人脸融合技术，将美妆产品的美妆效果呈现在用户脸上。

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
1. 用户在挑选口红时并不知道其上嘴的效果如何
2. 用户在想寻找相似妆容的口红产品却不知从何寻找，且想要同款口红
3. 美妆产品种类太多，且不知道其中的区别

**人工智能概率性**
- 人脸识别：腾讯云AI中的人脸识别api，人脸检测定位，可检测图片中的人脸并标记出人脸坐标，支持同时识别多张人脸。五官定位技术可以精准定位五官的位置，实现人脸美颜美妆、人脸变形、人脸漫画、人脸换脸、人脸贴纸等。基于人脸检测功能，可识别用户如年龄、性别、颜值等属性特征，对顾客画像自动分类，结合客户消费记录等信息，提供更精准的客群分层流量分析；同时结合产品促销信息，根据不同客群的属性，提供更生动的互动营销体验，提升顾客满意度，促进购物消费转化
- 人脸试妆api：基于腾讯优图领先的人脸识别算法，提供包括试唇色、测肤质、试妆容等多种功能，只需上传图片即可在线试妆，为用户提供高可用的人脸试妆服务。
- 人脸融合api：在美颜相机中，通过让用户上传两张人脸图片，实现对目标人脸进行美颜的目的，增加美颜功能的种类，提升用户体验。通过快速精准地定位人脸关键点，将用户上传的照片与特定形象进行面部层面融合，使生成的图片同时具备用户与特定形象的外貌特征
- 图像分析技术：可以识别出图片中的多个商品，并给出商品的品类、坐标，可以进行商品聚类、相似商品推荐，实现个性化广告展示，提高购买转化。

#### PRD5.需求列表与人工智能API加值 3%
需求列表：使用人工智能的加值是否反映到需求列表（核心功能的排序上）且PRD列出明显有可行及可用的API

  #|用户案例|重要性|技术
---|:------:|:-----|:-------
1|用户正在网上某购物平台挑选口红，但很苦恼不知道试在自己嘴上是什么效果|极其重要|人脸识别api和人脸试妆api
2|用户在网上看到某明星的妆容很好看，想知道其同款美妆产品、美妆教程及上脸效果|重要|人脸融合api和图像分析技术

---

## 原型 20%
#### 原型1.交互及界面设计 5%
交互及界面设计：在PRD文件中是否有说明且原型是否有做到：交互及界面设计的某个核心交互环节使用了人工智能的加值
![dd5409497107010ea9fd84b9635f643.png](https://upload-images.jianshu.io/upload_images/9513869-a87ddb75f114229b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  ![626f7a67c264b845e6fbc5b29dbdf72.png](https://upload-images.jianshu.io/upload_images/9513869-3890e71b7ffc5fba.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  ![a41f6e3e7be676e2cc079b5dac3a65d.png](https://upload-images.jianshu.io/upload_images/9513869-bd21ca13a9a41875.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![65b28dc38e6d97dcded4f5b1de8df0e.png](https://upload-images.jianshu.io/upload_images/9513869-26f73662111337ce.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240) ![fead8a08f2ba8c47bf137a08d7ba048.png](https://upload-images.jianshu.io/upload_images/9513869-777193cebc13098c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240) ![71a7314e300db59c34034c6b66896a5.png](https://upload-images.jianshu.io/upload_images/9513869-ad1404e6bdbc0992.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  

![1da292661b7f1853116149a4d423de3.png](https://upload-images.jianshu.io/upload_images/9513869-821c9fb6bf7d26bc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)




#### 原型2.信息设计 5%
信息设计：在PRD文件中是否有说明且原型是否有做到：信息设计的某个核心信息或设计使用了人工智能的加值
![产品架构.png](https://upload-images.jianshu.io/upload_images/9513869-727b4e20d7944e5b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 原型3.原型文档 5%
[口红试色app原型](http://nfunm085.gitee.io/api_axure)
[口红试色app原型下载](https://gitee.com/NFUNM085/api_axure)

#### 原型4.口头操作说明 5%

大家好，我们团队的项目做的是一款线上就能实现口红试色及购物的app。用户可以根据自己的需求，选择钟意的口红之后，打开摄像头就能看到试色效果，此功能运用了腾讯云中的人脸识别和人脸融合的技术，其识别功能精准，其中的五官定位技术可以精准定位五官的位置，实现人脸美颜美妆、人脸换脸、人脸贴纸等。融合技术自然高潮，其算法业界领先，经过人民日报军装照等大量的活动验证，融合效果自然，可以实现多种融合美颜功效。通过图像分析技术，用户只需拍摄或上传想要识别的图像中的口红颜色，此软件便可以识别出图片中相似口红并推荐给用户，并且会给出该口红的适合人群及肤色和搭配建议，对商品进行聚类、相似商品推荐，实现个性化广告展示，提高购买转化。

---

### API 产品使用关键AI或机器学习之API的输出入展示 15%
#### API1.使用水平 5%
使用水平：在PRD文件中是否有说明且展示，核心功能所应用的API之输入及输出
- 输入
- 示例1 调用返回成功（使用RGBA指定唇色）
```
https://fmu.tencentcloudapi.com/?Action=TryLipstickPic
&Image=xxxxx
&LipColorInfos.0.RGBA.R=200
&LipColorInfos.0.RGBA.G=0
&LipColorInfos.0.RGBA.B=0
&LipColorInfos.0.RGBA.A=50
&<公共请求参数>
```
- 输出
```
{
  "Response": {
    "ResultImage": "base64编码的图片",
    "RequestId": "3c140219-cfe9-470e-b241-907877d6fb03"
  }
}
```
- 示例2 调用返回成功（使用Lut素材modelid指定唇色）
- 输入
```
https://fmu.tencentcloudapi.com/?Action=TryLipstickPic
&Image=xxxxx
&LipColorInfos.0.ModelId=xxx
&<公共请求参数>
```
- 输出
```
{
  "Response": {
    "ResultImage": "base64编码的图片",
    "RequestId": "3c140219-cfe9-470e-b241-907877d6fb03"
  }
}
```

#### API2.使用比较分析 5%
使用比较分析：在PRD文件中是否有说明且提供连结证据，所使用的API是查找过最适用的（主要竞争者无或比较次），如考量其成熟度丶性价比丶等等

**性价比**

腾讯云
![6cc4049684b06eb6edcddfcd9fd3b16.png](https://upload-images.jianshu.io/upload_images/9513869-76e10e7bde95f48d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![c2c9d703c8b7ff55ccbd7503d58c126.png](https://upload-images.jianshu.io/upload_images/9513869-f20e05db701a9c55.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![e6224751ed2a8e4822fbbc85c62c80d.png](https://upload-images.jianshu.io/upload_images/9513869-9f6bfd84f959720e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![4a0be95fef40e1e85e5269d18e2907d.png](https://upload-images.jianshu.io/upload_images/9513869-608ebba1e96208c8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

百度ai
![7203559626cf78daec468f8de457d92.png](https://upload-images.jianshu.io/upload_images/9513869-df91bda51af4b12b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![0dcbd8416e99a458ed55c57203ea5fd.png](https://upload-images.jianshu.io/upload_images/9513869-2f0216bbf560a783.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### API3.使用后风险报告 5%
使用后风险报告：在PRD文件中是否有说明且提供连结证据，所使用的API类别的现在及未来发展性，如API市场竞争程度丶输入输出限制丶定价丶及可替代的程序库（改用自己开发的代码及数据库而不用API）等等

- 通过测试腾讯云的人脸识别技术达到99.80%，而百度ai达到96.20%;腾讯云每月每种服务均有10000次的免费调用额度，而百度ai该接口仅提供累计500次免费调用量，免费额度用尽后开始计费。



**人工智能概率性**
- 腾讯云的人脸识别具备高并发、高吞吐、低时延等特点，即使是百万规模人脸搜索，仍只需数百毫秒即可处理完毕，满足您的实时使用需求。五官定位技术可以精准定位五官的位置，实现人脸美颜美妆、人脸换脸、人脸贴纸等。 
- 腾讯云的人脸融合技术与优图实验室、天天P图联合打造的 AI 变脸玩法。通过快速精准地定位人脸关键点，将用户上传的照片与特定形象进行面部层面融合，使生成的图片同时具备用户与特定形象的外貌特征，支持单脸、多脸、选脸融合，满足不同的营销活动需求
#### API4.加分项 3%
使用复杂度：用了2个以上机器学习与人工智能的API之输入及输出
