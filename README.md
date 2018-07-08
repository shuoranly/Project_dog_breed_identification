[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## 项目概述

欢迎来到卷积神经网络（CNN）项目！在这一项目中，你将学到如何建立一个处理现实生活中的，用户提供的图像的算法。给你一个狗的图像，你的算法将会识别并估计狗的品种，如果提供的图像是人，代码将会识别最相近的狗的品种。

![Sample Output][image1]

在学习用于分类的最先进的 CNN 模型的同时，你将会为用户体验做出重要的设计与决定。我们的目标是，当你完成这一项目时，你将可以理解，通过将一系列模型拼接在一起，设计数据处理管道完成各式各样的任务所面临的挑战。每个模型都有它的优点与缺点，并且设计实际应用时，经常会面对解决许多没有最优解的问题。尽管你的解答不是最优的，但你的设计将带来愉快的用户体验！


## 项目指南

### 步骤

1. 克隆存储库并打开下载的文件夹。

 ```	
git clone https://github.com/udacity/cn-deep-learning.git
cd cn-deep-learning/dog-project
```

2. 下载[狗狗数据集](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd101/v4-dataset/dogImages.zip) ，并将数据集解压大存储库中，地点为`项目路径/dogImages`. 

3. 下载[人类数据集](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd101/v4-dataset/lfw.zip)。并将数据集解压大存储库中，位置为`项目路径/lfw `。

4. 为狗狗数据集下载 [VGG-16关键特征](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd101/v4-dataset/DogVGG16Data.npz) 并将其放置于存储库中，位置为`项目路径/bottleneck_features `。

5. 安装必要的 Python 依赖包


	对于 __Mac/OSX__：
	
	```bash
	conda env create -f requirements/dog-mac.yml
	source activate dog-project
	KERAS_BACKEND=tensorflow python -c "from keras import backend"
	```

	对于 __Windows__：
	
	```bash
	conda env create -f requirements/dog-windows.yml
	activate dog-project
	set KERAS_BACKEND=tensorflow
	python -c "from keras import backend"
	```
6. 打开 notebook

 ```
jupyter notebook dog_app.ipynb
```

__注意：__ 我们虽然已经实现了一些代码，让你更快地开始工作，你仍需要实现额外的功能，以回答 notebook 中所有的问题。
__除非有要求，否则不要修改任何已经包含的代码。__

