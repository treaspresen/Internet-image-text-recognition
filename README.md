我们对官方提供的训练集进行了处理，将其准换成yolo格式，训练集和官方测试集放在百度网盘中，地址：
运行步骤：
    1、在终端中输入 python train.py --epochs 50
    运行完后会在runs文件夹中生成运行时的相关文件，包括最优模型、超参数等。
    2、在终端中输入 python detect.py --weights runs/train/exp/weights/best.pt --save-txt
    也可以在train.py和detect.py中对相关参数进行修改。
    --save-txt会保存每张测试图片的检测结果坐标信息
