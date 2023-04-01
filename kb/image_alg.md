# 图像算法
> 目标：建立图像算法的知识体系
> 内容：用途、使用场景、简单原理

## 分割
### 传统
| 类型 | 算法 | 说明 |
| :-: | - | - |
| 聚类(阈值) | Otsu，GMM，FMM |  |
| 边缘 | Surf. Sift|  |
| 图论 | Graph Cut. Grab Cut |  |
| 区域 | Region Grow. 区域分裂。分水岭 |  |
| 能量泛函 | active contour model; geometric active contour model |  |

### AI
uNet based

## 检测
### 传统
### AI
1. RCNN based
1. 人体姿势估计
1. 分类和目标检测: ResNet18 、 MobileNetV1 / V2 、 SSD 、 YOLO 、 FasterRCNN
1. ImageNet预训练模型：Resnet18 、 AlexNet 、 squezenet 和 Resnet50

## 配准(融合)
1. 配准对象：点云-点云，图像-点云，点云-图像
1. ICP算法配准点云矩阵
1. 粗配准vs精配准

## SLAM

## other
* [裸眼3D](https://www.zhihu.com/question/386525244) : 双目摄像头的视差
* 医学图像后处理算法（如降噪，增强，超分，加速等）

### 三维重建
* Marching Cube
