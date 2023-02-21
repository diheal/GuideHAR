# 可穿戴传感器入门指南 (Wearable Sensor Starter Guide from Deep Learning Perspective for Human Activity Recognition)
 
## 1. 基础知识
目标：熟悉机器学习中监督学习和无监督学习的常用方法和概念；熟悉深度学习常用网络结构；掌握使用深度学习框架构建自定义模型，并完成分类或回归任务的训练。
| 课程 | 推荐课程 | 推荐书籍 | 目标 |
| -- | -- | -- | -- |
|Python 3 | | [[菜鸟教程]](https://www.runoob.com/python3/python3-tutorial.html) <br/> [[Python数据分析]](https://item.jd.com/12398725.html) | 熟悉Python基础逻辑语法，可以使用Python刷LeetCode。对Numpy和Pandas库有一定了解和应用。
|机器学习 | [[实用机器学习]](https://www.bilibili.com/video/BV13U4y1N7Uo) <br/> [[吴恩达机器学习课程]](https://www.bilibili.com/video/BV1LE411h7P4) | [[机器学习实战]](https://item.jd.com/12732035.html)| |
|深度学习| [[吴恩达深度学习课程]](https://www.bilibili.com/video/BV12E411a7Xn) <br/> [[Pytorch]](https://www.bilibili.com/video/BV1oX4y137bC) <br/> [[Tensorflow 2]](https://www.bilibili.com/video/BV1B7411L7Qt) <br/> [[北邮课程P4,5,6]](https://www.bilibili.com/video/BV1V54y1B7K3)|[[动手学深度学习纸字版](https://item.jd.com/13628339.html) [网页版](http://zh-v2.d2l.ai/)]
## 2. 监督学习
目标：在监督学习环境下完成活动分类任务的训练和评估，如DeepConvLSTM；熟练替换训练模型中的各个组件。

### 常用可穿戴传感器数据集
[[UCI-HAR]](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones) [[OPPORTUNITY]](https://archive.ics.uci.edu/ml/datasets/opportunity+activity+recognition) [[USC-HAD]](https://sipi.usc.edu/had/) [[SHAR]](http://www.sal.disco.unimib.it/technologies/unimib-shar/) [[HHAR]](http://archive.ics.uci.edu/ml/datasets/heterogeneity+activity+recognition) [[MotionSense]](https://github.com/mmalekzadeh/motion-sense/tree/master/data)

### 数据集(训练集，测试集）划分方式
按用户划分；随机划分

**需要注意实验是要求按用户分割还是随机划分训练集和测试集，可以参考相关工作中，相同实验的处理方式**
### 数据预处理代码
[[OPPORTUNITY]](https://github.com/STRCWearlab/DeepConvLSTM_py3) [[HHAR/SHAR/UCIHAR]](https://github.com/Tian0426/CL-HAR/tree/main/data_preprocess) [[UCI-HAR]](https://blog.csdn.net/bucan804228552/article/details/125118832) [[MotionSense]](https://github.com/iantangc/ContrastiveLearningHAR)

### 模型构建与训练
完成DeepConvLSTM模型的构建与训练 [[paper]](http://www.mdpi.com/1424-8220/16/1/115/html) [[code1]](https://github.com/STRCWearlab/DeepConvLSTM_py3) [[code2]](https://github.com/Tian0426/CL-HAR)；并在多种数据集上训练和评估该模型。