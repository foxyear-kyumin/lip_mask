# LIP_MASK：具有地标和外观先验的保持身份的说话人脸生成（CVPR 2023）

CVPR2023论文“**I**dentity-**P**reserving Talking Face Generation with **L**andmark and **A**ppearance **P**riors” 的PyTorch官方方案的升级。

[[论文]](https://arxiv.org/abs/2305.08293) [[演示视频]](https://youtu.be/wtb689iTJC8)

## 如何实现效果的提升？
- 通过dlib优化关键点检测方式
- 对齐音频视频帧
- 二次生成说话脸速度提升
- 通过锐化滤波加强清晰度

## 环境要求
- Python 3.9
- torch  2.0.0
- torchvision 0.15.1
- ffmpeg

我们在1个24G的RTX3090上使用CUDA 118进行实验。更多细节，请参考 `requirements.txt`。我们建议首先安装[pytorch](https://pytorch.org/)，然后运行以下命令：
```
pip install -r requirements.txt
```

## 测试
从[OneDrive](http://cloud.foxyear.cn/s/jMtW)下载预训练模型,密码'foxyear'，并将其放置在 `checkpoints` 文件夹中。然后运行以下命令：
```
python inference.py
```

## 运行
从[OneDrive](http://cloud.foxyear.cn/s/jMtW)下载预训练模型,密码'foxyear'，并将其放置在 `checkpoints` 文件夹中。然后运行以下命令：
```
python inference.py  --input ./video/videoxx.mp4 --audio ./audio/testxx.wav
```

## 致谢
该项目在公开可用的代码 [IP_LAP](https://github.com/Weizhi-Zhong/IP_LAP) , [DFRF](https://github.com/sstzal/DFRF) , [pix2pixHD](https://github.com/NVIDIA/pix2pixHD), [vico_challenge](https://github.com/dc3ea9f/vico_challenge_baseline/tree/a282472ea99a1983ca2ce194665a51c2634a1416/evaluations) 和 [Wav2Lip](https://github.com/Rudrabha/Wav2Lip/tree/master) 基础上构建而成。感谢这些作品和代码的作者将他们优秀的工作公开发布。


## 联系
深度开发合作交流，联系加微信：

<img src='./2.jpg' width=200>

交流群及资料教程：

<img src='./1.jpg' width=200>


## 引用和点赞
如果你在研究中使用了这个库，请引用以下论文并为该项目点赞。谢谢！
```
@InProceedings{Zhong_2023_CVPR,
    author    = {Zhong, Weizhi and Fang, Chaowei and Cai, Yinqi and Wei, Pengxu and Zhao, Gangming and Lin, Liang and Li, Guanbin},
    title     = {Identity-Preserving Talking Face Generation With Landmark and Appearance Priors},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2023},
    pages     = {9729-9738}
}
```
