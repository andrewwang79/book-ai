# 图像算法
> 目标：建立图像算法的知识体系
> 内容：用途、使用场景、简单原理

## 预处理
> 重采样，归一化

## 分割
### 传统
| 类型 | 算法 | 说明 |
| :-: | - | - |
| 聚类(阈值) | Otsu，GMM，FMM |  |
| 边缘 | Surf. Sift|  |
| 图论 | Graph Cut. Grab Cut |  |
| 区域 | Region Grow. 区域分裂。分水岭 |  |
| 能量泛函 | active contour model; geometric active contour model |  |

### 分割应用的算法
| 名称 | 说明 |
| :-: | - |
| Threshold | 阈值法分割 |
| Margin | 现有分割结果向外生长或者收缩特定像素 |
| Hollow | 现有分割结果中间掏空，用在血管壁的分割比较管用 |
| Grow from seeds |  |
| Level Tracing | 根据灰度值在平面内生成一个轮廓 |
| Fill between slices | 自动在切片之间进行插值填充，不用在每一slice进行标注，只标注关键slice然后自动插值填充再微调即可 |

### AI
> uNet based
> 检测、分割和定位：聚类和概率筛选
* [图像多label分割](https://blog.csdn.net/jancis/article/details/106209808)

## 检测
### 传统
### AI
1. RCNN based
1. 人体姿势估计
1. 分类和目标检测: ResNet18 、 MobileNetV1 / V2 、 SSD 、 YOLO 、 FasterRCNN
1. ImageNet预训练模型：Resnet18 、 AlexNet 、 squezenet 和 Resnet50

## 配准
* [医学图像配准技术综述](https://zhuanlan.zhihu.com/p/267339046)
* [3DSlicer多模态图像配准教程](http://www.360doc.com/content/22/0311/11/66272086_1021038063.shtml)
* [3DSlicer下图像的配准与融合（一）单模态图像的配准和融合](http://www.medtion.com/info/18758.jspx)
* 配准对象：点云-点云，图像-点云，点云-图像
* 粗配准vs精配准

### 刚性配准
> 给定两个点集，刚性配准会产生一个刚性变换矩阵，该变换矩阵将一个点集映射到另一个点集上，刚性变换定义为不改变任何两点之间距离的变换，一般这种变换只包括平移和旋转。
在术中导航中，刚性配准常通过在CT和患者身上都存在且明确可辨的点进行配准，常用植入骨内的配准钉、明确的解剖标志点例如支气管的隆突点。

* ICP配准算法
    1. 首先进行粗配准，初始化旋转平移矩阵  
    1. 对两组点集寻找最近对应点
    1. 根据对应点利用SVD分解计算新的旋转平移矩阵
    1. 对点集进行旋转平移变换，得到的新点集再和目标点集计算对应点
    1. 重复2-4，直到迭代次数或者变化量达到阈值

* [矩阵奇异值分解（SVD）](https://zhuanlan.zhihu.com/p/480389473)

## SLAM

## other
* [裸眼3D](https://www.zhihu.com/question/386525244) : 双目摄像头的视差
* 医学图像后处理算法（如降噪，增强，超分，加速等）

### 三维重建
* Marching Cube
