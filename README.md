## 本仓库介绍
为了备战 [ICME-2022 安全AI挑战者计划第九期：小样本商标检测挑战赛](https://tianchi.aliyun.com/competition/entrance/531948/introduction)，当前工作和未来工作计划:
已完成工作:

* 基于开源的openbrand数据集制作了LogDetMini 数据集，基于coco格式，并开源
* 基于LogDetMini进行数据可视化分析 `LogDetMini/eda/eda.ipynb`
* 基于mmdetection进行baseline实验和基础调参实验
* 初赛 ContestStage1 的 eda `ContestStage1/eda/logdet-eda.ipynb`
* 进行baseline实验 

未来工作计划:
* 继续调优

欢迎在issue区讨论

## 初赛实验(ContestStage1)

为方便实验对比，本地划分了0.2作为 val，见 `ContestStage1/data`

|         方案         |  本地val  |  线上  | Training time/h |
| :------------------: | :---: | :-------------: | :-------------: |
|         swinb_3x_bigsize_anchor_bs2x8         | 0.591 | 0.5114 |       1.5      |





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

正式赛开始后，感觉和构建的 mini 数据集有一定区别，LogDetMini 移到[这里](https://github.com/CarryHJR/LogDet/tree/master/LogDetMini)

<!-- ![](https://tva1.sinaimg.cn/large/e6c9d24egy1h0td1awfjyj20u00ur0yy.jpg) -->

