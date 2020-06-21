### 学院：计算机学院&emsp;学号：3220190894&emsp;姓名：吴嘉豪
# 互评作业4: 离群点分析与异常检测
**问题描述：**
- 本次作业将从Anomaly Detection Meta-Analysis Benchmarks提供的benchmark数据集中任选两个进行分析。
------------

**使用的Dataset：**
- [Anomaly Detection Meta-Analysis Benchmarks](https://ir.library.oregonstate.edu/concern/datasets/47429f155?locale=en)
- Dataset - **Skin**
- Dataset - **pageb**
------------

**使用的环境：**
- 使用了Python Outlier Detection (PyOD)完成分析工作
```python
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
from sklearn.utils import shuffle

from pyod.models.pca import PCA
from pyod.models.knn import KNN
from pyod.models.lof import LOF
from pyod.models.iforest import IForest

from time import *
import sys
import os

from sklearn.metrics import roc_auc_score
from sklearn.utils import column_or_1d
from sklearn.utils import check_consistent_length
from pyod.utils.utility import precision_n_scores

import warnings
```

------------

**仓库文件介绍：**
- **分析过程报告**：
	- homeworkw4.html为数据集的分析过程报告；
- **程序**：
	- homeworkw4.ipynb为对应的python notebook过程代码；

