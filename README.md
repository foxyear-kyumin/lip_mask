# IP_LAP: Identity-Preserving Talking Face Generation with Landmark and Appearance Priors （CVPR 2023）

Pytorch official implementation for our CVPR2023 paper "**I**dentity-**P**reserving Talking Face Generation with **L**andmark and **A**ppearance **P**riors".

<img src='./CVPR2023framework.png' width=900>

TODO:
- [x] Demo videos
- [x] pre-trained model
- [x] code for testing
- [x] code for training
- [x] code for preprocess dataset
- [x] guideline 
- [x] arxiv paper release

[[Paper]](https://arxiv.org/abs/2305.08293) [[Demo Video]](https://youtu.be/wtb689iTJC8)

## Requirements
- Python 3.9
- torch  2.0.0
- torchvision 0.15.1
- ffmpeg

We conduct the experiments with 4 24G RTX3090 on CUDA 118. For more details, please refer to the `requirements.txt`. We recommend to install [pytorch](https://pytorch.org/) firstly, and then run:
```
pip install -r requirements.txt
```
## Test
Download the pre-trained models from [OneDrive](http://cloud.foxyear.cn/s/jMtW) and place them to the folder `checkpoints` . Then run the following command:
```
CUDA_VISIBLE_DEVICES=0 python inference.py
```


## Acknowledgement
This project is built upon the publicly available code [IP_LAP](https://github.com/Weizhi-Zhong/IP_LAP) , [DFRF](https://github.com/sstzal/DFRF) , [pix2pixHD](https://github.com/NVIDIA/pix2pixHD), [vico_challenge](https://github.com/dc3ea9f/vico_challenge_baseline/tree/a282472ea99a1983ca2ce194665a51c2634a1416/evaluations) and [Wav2Lip](https://github.com/Rudrabha/Wav2Lip/tree/master). Thank the authors of these works for making their excellent work and codes publicly available.


## Citation and Star
Please cite the following paper and star this project if you use this repository in your research. Thank you!
```
@InProceedings{Zhong_2023_CVPR,
    author    = {Zhong, Weizhi and Fang, Chaowei and Cai, Yinqi and Wei, Pengxu and Zhao, Gangming and Lin, Liang and Li, Guanbin},
    title     = {Identity-Preserving Talking Face Generation With Landmark and Appearance Priors},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2023},
    pages     = {9729-9738}
}




