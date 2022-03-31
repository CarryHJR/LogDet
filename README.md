## 本仓库介绍
为了备战 [ICME-2022 安全AI挑战者计划第九期：小样本商标检测挑战赛](https://tianchi.aliyun.com/competition/entrance/531948/introduction)，当前工作和未来工作计划:
当前工作:

* 基于开源的openbrand数据集制作了LogDetMini 数据集，基于coco格式，并开源
* 基于LogDetMini进行数据可视化分析 `LogDetMini/eda/eda.ipynb`
* 基于mmdetection进行baseline实验和基础调参实验

未来工作计划:
* 在赛事数据集发布后(4.11)，基于正式数据集，进行eda和baseline实验 


## LogDetMini数据集
下载地址: https://pan.baidu.com/s/1fg9IaPh061iD7w5aiIX3qg?pwd=m3gm
```
.
├── class_names.txt
├── images
├── instances_train2017.json
└── instances_val2017.json

```
简单介绍: 从openbrand数据模拟复赛分布，随机选取了50类，每类20张作为train, 20张作为val，train和val之间数据不重复

![](https://tva1.sinaimg.cn/large/e6c9d24egy1h0td1awfjyj20u00ur0yy.jpg)

## LogDetMini 实验

|         方案         |  mAP  | Training time/h |
| :------------------: | :---: | :-------------: |
|         r101         | 0.344 |       0.4       |
|       r101_3x        | 0.447 |        \        |
|     r101_3x_flip     | 0.455 |        \        |
| r101_3x_flip_softnms | 0.457 |        \        |
|       r101_12x       | 0.452 |       1.5       |

