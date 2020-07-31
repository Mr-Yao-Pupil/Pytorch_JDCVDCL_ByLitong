### 实现的内容

-  主干特征提取网络：目前只调用了ResNet50
-  训练用到的小技巧：学习率衰减
-  激活函数：作者的其他函数暂未复现使用

### 编码环境

torch==1.5.0

### 注意事项

还没想到

### 小技巧的设置

1. 中途终止训练直接停止代码，若要接着训练更改Train.py文件中的premodulepath地址为已经保存的模型即可

### 文件下载

在执行时会自动从官方的预训练的模型下载参数

### 预测步骤

#### 1、使用预训练权重

1. 在cfg.py文件中更改预训练权重的本地路径，具体参看pytorch官方文档路径
2. 将所有的图片按照分类放入文件夹：data_img
3. 通过Generate_TXT.py生成标签文件，由于代码还未封装，故需要根据自己的分类复制粘贴一下。嘻嘻

#### 2、运行train.py即可开始训练。
