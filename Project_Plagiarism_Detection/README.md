# 剽窃项目 - 机器学习部署

此代码库包含使用 AWS SageMaker 部署剽窃检测器的代码和相关文件。

## 项目概述

在此项目中，你需要构建一个剽窃检测器，它会检测文本文件并进行二元分类：根据文本文件与提供的原文之间的相似度，将文件标为*剽窃文件*或*非剽窃文件*。检测剽窃行为是一个很活跃的研究领域；这项任务比较有挑战性，因为剽窃文件与原文之间的区别通常并不明显。

此项目将分成三个主要 notebook：

**Notebook 1：数据探索**
* 加载剽窃文本数据的语料库。
* 探索现有的数据特征和数据分布
* 最终提交项目时**不**需要提交第一个 notebook。

**Notebook 2：特征提取**

* 清理和预处理文本数据。
* 定义用于比较答案和原文之间相似性的特征，并提取相似性特征
* 通过分析不同特征之间的相关性，选择“合适的”特征。
* 创建训练/测试 `.csv` 文件，其中包含训练/测试数据点的相关特征和类别标签。

**Notebook 3：在 SageMaker 中训练和部署模型**

* 将训练/测试特征数据上传到 S3。
* 定义二元分类模型和训练脚本。
* 使用 SageMaker 训练和部署模型。
* 评估部署的分类器。 

---

请参阅根目录下的 [README](https://github.com/udacity/ML_SageMaker_Studies/tree/master/README.md)，了解如何设置 SageMaker notebook 并下载项目文件（及其他 notebook）。

