## TireNet —— A method for tire track image recognition
![image](https://github.com/user-attachments/assets/ea532797-e853-4d57-8afb-c8550205ce4c)

## 环境要求
matplotlib==3.7.4
matplotlib-inline==0.1.6
mdurl==0.1.2
mmcls==0.23.0
mmcv-full==1.5.2
mmdet==2.24.1
numpy==1.24.4
## 创建环境
conda create -n tire python=3.8.2 -y
conda activate tire
## 安装基础环境
pip install -r requirement.txt #安装基础环境
## 搭建环境
cd tire_recognition_CAMN
pip install -r requirements/build.txt
pip install -v -e .  # or "python setup.py develop"

## 训练过程(5way1shot训练为例)
python tools/classification/train.py configs/classification/matching_net/mini_imagenet/matching-net_resnet12_1xb105_mini-imagenet_5way-1shot.py 

## 测试过程(5way1shot训练为例)
python tools/classification/test.py configs/classification/matching_net/mini_imagenet/matching-net_resnet12_1xb105_mini-imagenet_5way-1shot.py --metric Recall

参考代码库如下，非常感谢openmmlab社区的贡献。
https://github.com/open-mmlab/mmfewshot

