### 一、数据集

​	我们对官方提供的训练集进行了处理，将其准换成yolo格式，训练集和官方测试集放在百度网盘中，

地址： https://pan.baidu.com/s/1qaGIDDEoC_huAN5LChXECQ?pwd=x8bt

将其中的images、images_test、labels三个文件夹放在data文件夹下

预处理代码在precode文件夹中

### 二、运行步骤： 

#### 1、训练

​	在终端中输入 `python train.py --epochs 50` 运行完后会在runs文件夹中生成运行时的相关文件，包括最优模型、超参数等。 

​	官方的预训练模型yolov7.pt放在百度网盘，地址：https://pan.baidu.com/s/1JPUsEMNzDJLCI_UklJyJ5g?pwd=oqd2

​	我们训练50个epoch的模型，百度网盘地址：https://pan.baidu.com/s/1rWo5uA_kRXpkN7YaLVQB-Q?pwd=vucy

​	（建议将模型直接放在主文件夹）

#### 2、测试（检测）

​	在终端中输入 `python detect.py --weights runs/train/exp/weights/best.pt --save-txt` 

也可以在train.py和detect.py中对相关参数进行修改。 --save-txt会保存每张测试图片的检测结果坐标信息。