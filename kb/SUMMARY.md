# AI
## 深度学习
* 常见的神经网络操作：矩阵乘法、卷积、池化、归一化等
* 超参数：在机器学习和深度学习中用于控制模型训练过程的参数，在训练之前手动设置。超参数的选择可以对模型的性能和训练过程产生重要影响。常见超参数如批量大小（Batch Size），学习率（Learning Rate）
* 下采样（Downsampling）：一种降低数据维度或减少数据量的方法。在机器学习和信号处理中经常使用下采样来处理高维数据或减少数据样本数量，以减少计算复杂度或解决数据不平衡的问题。

### 网络类型
* 分类: https://zhuanlan.zhihu.com/p/159305118

| 类型 | 网络 | 说明 |
| - | - | - |
| 卷积神经网络（Convolutional Neural Networks，CNN） | AlexNet，ResNet，UNet | 图像分割和识别。处理图像和视觉任务。卷积层和池化层来有效地提取图像中的特征，通过全连接层进行分类或回归。卷积层通过卷积操作对输入进行特征提取，池化层用于降采样和特征压缩，全连接层用于将提取的特征映射到输出类别上。 |
| Transformer | GPT（Generative Pre-trained Transformer） | 基于注意力机制的网络（Attention-Based Networks），特别适用于处理序列数据，广泛应用于自然语言处理任务。最初用于自然语言处理任务，如机器翻译。在处理序列数据时取得了重大突破，成为自然语言处理任务的标准模型。由编码器和解码器组成。编码器和解码器都由多个层堆叠而成，每个层包含多头自注意力机制和前馈神经网络。 |
| 前馈神经网络（Feedforward Neural Networks，FNN） | 多层感知机（Multilayer Perceptron，MLP） |  |
| 循环神经网络（Recurrent Neural Networks，RNN） |  |  |

### 常用层
1. 全连接层（Fully Connected Layer）：也称为密集连接层或线性层，每个神经元都与上一层的所有神经元相连接。它用于学习输入数据的复杂非线性关系，常用于分类和回归任务。
1. 卷积层（Convolutional Layer）：通过卷积操作对输入数据进行特征提取。卷积层在计算机视觉领域广泛应用，用于图像处理和对象识别等任务。
1. 池化层（Pooling Layer）：通过降采样操作减小特征图的空间尺寸，减少计算复杂度并提取最显著的特征。常见的池化操作包括最大池化和平均池化。
1. 规范化层（Normalization Layer）：如批量归一化（Batch Normalization）和层归一化（Layer Normalization），用于加速训练过程、增加模型的稳定性和减少内部协变量偏移。

### 激活函数
* https://zhuanlan.zhihu.com/p/352668984，https://zhuanlan.zhihu.com/p/337902763, https://blog.csdn.net/wjinjie/article/details/104729911
* 使用非线性激活函数是为了增加神经网络模型的非线性因素。激活函数对于人工神经网络模型去学习、理解非常复杂和非线性的函数来说具有十分重要的作用。
* 常用激活函数
    1. Sigmoid函数（Logistic函数）：将输入值压缩到0到1之间的连续范围，公式为 f(x) = 1 / (1 + exp(-x))。
    1. ReLU函数（Rectified Linear Unit）：对于正输入，输出为输入值本身；对于负输入，输出为0，公式为 f(x) = max(0, x)。
    1. Softmax函数：常用于多类别分类问题，将输入映射为概率分布，使得所有输出值之和等于1。

### 卷积核
* 影响到网络的性能和学习能力。初始权重通常使用随机初始化的方法，如高斯分布或均匀分布。合适的初始化方法可以帮助网络更快地收敛和更好地学习特征。

### 模型
* 压缩技术：量化剪枝

### 梯度下降
* 暴力调优

### 组件
* 编码器，解码器：将输入数据转换成一种中间表示（编码）和将这种中间表示转换回原始数据或目标数据（解码）。编码是数据的特征提取和压缩的结果

## 资料
### 机器学习
* **[斯坦福大学公开课 ：机器学习课程_全20集](http://open.163.com/special/opencourse/machinelearning.html)**
* [初学者必读：从迭代的五个层面理解机器学习](http://it.sohu.com/20161229/n477271597.shtml)
* [数据分析扫盲 -- 1.传统数据分析](https://www.zybuluo.com/heavysheep/note/636770)
* [数据分析扫盲 -- 2.机器学习](https://www.zybuluo.com/heavysheep/note/639120)

### 深度学习
* [寒武纪课程](https://developer.cambricon.com/index/curriculum/index/classid/7.html)
* [2016年不可错过的21个深度学习视频、教程和课程](https://zhuanlan.zhihu.com/p/24362823?utm_source=wechat_session&utm_medium=social)
* [初学者入门指南：深度学习的五级分类](http://www.dlworld.cn/ShenDuXueXiYingYong/2764.html)
* [程序员实用深度学习免费课程：从入门到实践](http://it.sohu.com/20161229/n477271598.shtml)
* [九本不容错过的深度学习和神经网络书籍](http://it.sohu.com/20161229/n477271599.shtml)
* [2016AI巨头开源IP盘点 50个最常用的深度学习库](https://news.cnblogs.com/n/559753/)

### 神经网络
* [卷积神经网络原理](https://www.zhihu.com/question/34681168)
* [卷积神经网络学习](https://blog.csdn.net/wjinjie/article/details/105016766)
* [感知机](https://zhuanlan.zhihu.com/p/492867531)