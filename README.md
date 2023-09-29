# Jittor挑战热身赛（手写数字生成赛题）

运行结果示例（https://s3.bmp.ovh/imgs/2023/04/24/b4954e69f71b0fca.png）

## 简介

本项目包含了第二届计图挑战赛计图 - 手写数字生成赛题的代码实现。本项目的特点是：采用了 Conditional GAN 方法对图片数据集MNIST处理，取得了生成特定数字的图像的效果。

## 安装 

本项目可在Ubuntu虚拟机8G内存上运行，训练时间约为 1 小时。

#### 运行环境
- ubuntu 20.04 LTS
- python >= 3.7
- jittor >= 1.3.0

#### 安装依赖
执行以下命令安装 python 依赖
```
pip install -r requirements.txt
```

#### 预训练模型
无需预训练模型模型。


## 训练

训练得到结果可运行以下命令：
```
bash python3 CGAN.py
```

## 推理

通过修改计算真实类别和虚假类别的损失函数，训练判别器成功分类手写数字，并为指定的数字序列生成相应的手写数字图片。

## 致谢

此项目基于论文 *Conditional Generative Adversarial Nets* 实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。