实验环境 4卡3090

基于mmdetection 2.14 

将 logdet_mini.py 放到 `mmdetection-2.14.0/mmdet/datasets` 下

在 `mmdetection-2.14.0/mmdet/datasets/__init__.py` 加入
```
from .logdet_mini import LogDetMini
```
