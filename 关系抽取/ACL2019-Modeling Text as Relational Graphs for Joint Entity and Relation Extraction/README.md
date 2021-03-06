# Modeling Text as Relational Graphs for Joint Entity and Relation Extraction
- 将文本建模为关系图用于关系提取
- 提取实体和语义关系是从非结构化文本构建知识结构的核心任务，传统的流水线方法通常是先进行命名实体识别然后对实体关系进行预测，联合学习实体识别和关系抽取能获得更好的效果，但这些联合模型需要进行大量的特征工程。已有的神经网络方法都不是端到端的联合模型，他们假设已知命名实体并预期现实世界的命名实体识别会导致模型表现显著降低。
- 本文提出了一个端到端的关系提取模型GraphRel，使用GCN和Bi-LSTM编码器学习抽取命名实体及关系，考虑了线性和依赖结构，以及文本的所有单词对之间的隐式特征；通过端到端的实体、关系联合建模，同时对所有实体对进行预测；也考虑到了实体和关系之间的相互作用

- [代码](https://github.com/tsujuifu/pytorch_graph-rel)