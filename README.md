任务描述

 

本次比赛是chip2019中的评测任务二，由平安医疗科技主办。chip2019会议详情见链接：http://cips-chip.org.cn/evaluation

 

迁移学习是自然语言处理中的重要一环，其主要目的是通过从已学习的相关任务中转移知识来改进新任务的学习效果，从而提高模型的泛化能力。

 

本次评测任务的主要目标是针对中文的疾病问答数据，进行病种间的迁移学习。具体而言，给定来自5个不同病种的问句对，要求判定两个句子语义是否相同或者相近。所有语料来自互联网上患者真实的问题，并经过了筛选和人工的意图匹配标注。

 

文件说明

 

给参赛选手的文件由train.csv、dev.csv、test.csv三个文件构成，train.csv是训练集，包含2万对人工标注好的疾病问答数据，由5个病种构成，其中diabetes10000对，hypertension、hepatitis、aids、breast_cancer各2500对。dev.csv是验证集，包含10000对无label的疾病问答数据，由5个病种构成，其中diabetes，hypertension、hepatitis、aids、breast_cancer各2000对。test.csv是测试集，包含5万对人工标注好的疾病问答数据，其中只有部分数据供验证。

 

category表示问句对的病种名称，分别对应：diabetes-糖尿病，hypertension-高血压，hepatitis-乙肝，aids-艾滋病，breast_cancer-乳腺癌。label表示问句之间的语义是否相同。若相同，标为1，若不相同，标为0。其中，训练集label已知，验证集和测试集label未知。

 

示例​

 

​问句1:糖尿病吃什么？

问句2:糖尿病的食谱？

label:1

 

问句1:乙肝小三阳的危害？

问句2:乙肝大三阳的危害？

label:0

 

训练集和验证集会在比赛开始后发布，测试集会在比赛结束前2天发布。具体时间请以主办方通知为准。
