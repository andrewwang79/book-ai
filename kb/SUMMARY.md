# 知识

* [人工智能、机器学习、深度学习与神经网络](https://zhuanlan.zhihu.com/p/86794447)
* [寒武纪课程](https://developer.cambricon.com/index/curriculum/index/classid/7.html)

## 基础知识
* 最小二乘法：最小平方
* [方差标准差协方差](https://www.cnblogs.com/xunziji/p/6772227.html)
* [信息熵](http://baike.baidu.com/item/%E4%BF%A1%E6%81%AF%E7%86%B5)：系统有序化程度，越有序越低
* [标量、向量、矩阵、张量](https://easyai.tech/ai-definition/scalar/)
* [梯度与法向量](https://zhuanlan.zhihu.com/p/62718992)
* 卷积

## 混淆矩阵(Confusion Matrix)
* ![混淆矩阵](../s/ai/confusionMatrix.png)
* https://cloud.tencent.com/developer/article/1527943
* https://blog.csdn.net/Orange_Spotty_Cat/article/details/80520839

>precision=查准率
灵敏度=recall，查全率
查准率=选出的样本中有多少比例样本是正例（期望样本）
查全率=有多少比例的正样本（期望样本）被选出来了

*指标分母=0的结果，逻辑参考自sklearn

| 指标 | 结果 | 场景 |
| :-: | - | - |
| 准确率 | 0 | 没有数据 |
| 精确率 | 0 | 没有预测的阳性数据 |
| 灵敏度 | 0 | 没有真实的阳性数据 |
| 特异度 | 0 | 没有真实的阴性数据 |

### ROC和AUC(Area under Curve)
* ROC是曲线，AUC是ROC曲线下的面积
* https://www.cnblogs.com/dlml/p/4403482.html

## 机器学习
* **[斯坦福大学公开课 ：机器学习课程_全20集](http://open.163.com/special/opencourse/machinelearning.html)**
* [初学者必读：从迭代的五个层面理解机器学习](http://it.sohu.com/20161229/n477271597.shtml)
* [数据分析扫盲 -- 1.传统数据分析](https://www.zybuluo.com/heavysheep/note/636770)
* [数据分析扫盲 -- 2.机器学习](https://www.zybuluo.com/heavysheep/note/639120)

## 深度学习
* [2016年不可错过的21个深度学习视频、教程和课程](https://zhuanlan.zhihu.com/p/24362823?utm_source=wechat_session&utm_medium=social)
* [初学者入门指南：深度学习的五级分类](http://www.dlworld.cn/ShenDuXueXiYingYong/2764.html)
* [程序员实用深度学习免费课程：从入门到实践](http://it.sohu.com/20161229/n477271598.shtml)
* [九本不容错过的深度学习和神经网络书籍](http://it.sohu.com/20161229/n477271599.shtml)
* [2016AI巨头开源IP盘点 50个最常用的深度学习库](https://news.cnblogs.com/n/559753/)

### 神经网络
* [卷积神经网络原理](https://www.zhihu.com/question/34681168)
* [卷积神经网络学习](https://blog.csdn.net/wjinjie/article/details/105016766)
* [激活函数](https://blog.csdn.net/wjinjie/article/details/104729911)
