## 写在前面的话

今天开始，做第一个系列视频，**《从零开始前后端react+flask》**，命名为A系列，系列教程将从英文字母A-Z不等）。<br/>
**未经允许，禁止转发，或用作商业用途**。（需非商业转载请联系作者，并表明出处）<br/>
一个小节尽量不要太长，采用b站直播+录制视频的形式。<br/>
教程来源：均以本人实际接触的项目和学习经历为主，可能比较多比较杂，适合不同能力不同等级的人。<br/>
**免费学习**（至少现阶段是），不能保证每个知识点都正确或精通，但**能保证认真观看绝对有收获。**<br/>
不敢说一直坚持下去做多久，希望能在大家的支持下走的更远。<br/>
目的：一方面，对自己学习的知识总结，和提高表达沟通能力；一方面，能把自己学到的知识分享给大家，也是一种有意义的事。<br/>

<br/>
B站：https://space.bilibili.com/51723516<br/>
csdn：https://blog.csdn.net/GreatXiang888<br/>
github：https://github.com/JizhiXiang<br/>
适用人群：理工类在校大学生，研究生，对编程感兴趣，学过至少一门编程语言，自控力一般的童鞋。 进群早且有空的朋友，可以申请群管理。 <br/>
up主简介，北京某985研三在读，某互联网大厂offer，人工智能NLP方向。 <br/>
侧重点：自然语言处理，机器学习，算法，有意思的脚本，简单的前后端，区块链技术，量化交易 <br/>
群宗旨：一起学编程，分享学习经验，只有真本事才有竞争力。<br/>
短期想法是，直播编程学习，如果有时间，会对自己学习的东西做一个总结，争取做出一些有价值且好理解的教学视频。<br/>
<br/>

---- 

## 技术介绍

首先说一点，我做的可能和一般的教程不一样，有过百度搜索编程经验的同学都知道，**很多网上教程都是抄来抄去，而且都是一些简单的demo，意义不大，对初学者很不友好**，而国外的网址又上不去或者英文看不懂。我也是花了很多时间，踩了很多坑，最后才实现自己想要的功能；再把它总结起来，作为一个教程，希望新来的人少走一些弯路。另外，我按照自己的思路来讲，不拘泥于传统步骤，要用到什么讲什么，最终肯定能实现目标。<br/>


先熟悉一下相应的技术名词：**react，flask，python，sqlite，js，antdesign，Axure**就在一两个月前，老师问我会不会做一个web版的应用，界面不要太丑。我说不会，但我可以学。他说，那你用antdesign和python搭吧，去学一学。<br/>
emmm，然后现在感觉学到一些了，如下。<br/>
<br/>
（我的理解）
==js==：编程语言，全称JavaScript，和java没关系，和一些动态操作，逻辑处理相关，是web设计的灵魂。 百度百科[https://baike.baidu.com/item/javascript/321142 ](https://baike.baidu.com/item/javascript/321142)<br/>
==react==: 用于构建用户界面的 JavaScript 库，比较好用的一种js，传统的js比较老写起来麻烦。react官网 [https://react.docschina.org/](https://react.docschina.org/)<br/>
==antdesign==: 蚂蚁金服开发的一套组件，和react结合使用，非常漂亮，且简单。官网 [https://ant.design/index-cn](https://ant.design/index-cn)
上面这些技术是前端用的，就是展示在网页上。但如果要对数据进行处理，添加算法，或存储，需要后端。
<img src="https://img-blog.csdnimg.cn/2019112710380755.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0dyZWF0WGlhbmc4ODg=,size_16,color_FFFFFF,t_70" width="80%" height="80%" alt=""/>
(ps:通过自己写img标签来修改上传图片大小)<br/>
==Axure==： 是一款专业的快速原型设计工具。用来做UI界面，适合产品经理。 百度百科[https://baike.baidu.com/item/axure%20rp/9653646](https://baike.baidu.com/item/axure%20rp/9653646)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191127112216838.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0dyZWF0WGlhbmc4ODg=,size_16,color_FFFFFF,t_70)<br/>
==python==：编程语言，用来写后端，有很多现成的库，完全开源，使用简单方便，必不可少的技术，强推。百度百科[https://baike.baidu.com/item/python/407313](https://baike.baidu.com/item/python/407313)<br/>
==flask==：是一个使用 Python 编写的轻量级 Web 应用框架。可以用python搭网站，简单实用。百度百科[https://baike.baidu.com/item/Flask](https://baike.baidu.com/item/Flask)<br/>
==sqlite==：是一款轻型的数据库，用python操作起来非常简单。百度百科 [https://baike.baidu.com/item/SQLite/375020](https://baike.baidu.com/item/SQLite/375020)<br/>


## 我们的目标
要做出一个**完整的前后端系统，拥有增删改查功能，存储功能，管理员权限，上传文件等，且界面优美。**<br/>

![在这里插入图片描述](https://img-blog.csdnimg.cn/20191127140438777.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0dyZWF0WGlhbmc4ODg=,size_16,color_FFFFFF,t_70)
<br/>


