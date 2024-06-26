# tire_recognition_CAMN
![f36ea31f42fdbf5da269172d36eef47](https://github.com/hejinrong/tire_recognition_CAMN/assets/10822423/1f03892d-7f79-49a1-be63-762f3eaec0a6)

# 环境要求
matplotlib==3.7.4
matplotlib-inline==0.1.6
mdurl==0.1.2
mmcls==0.23.0
mmcv-full==1.5.2
mmdet==2.24.1
numpy==1.24.4
# 创建环境
conda create -n tire python=3.8.2 -y
conda activate tire
# 安装基础环境
pip install -r requirement.txt #安装基础环境
# 搭建环境
cd tire_recognition_CAMN
pip install -r requirements/build.txt
pip install -v -e .  # or "python setup.py develop"

# 训练过程(5way1shot训练为例)
python tools/classification/train.py configs/classification/matching_net/mini_imagenet/matching-net_resnet12_1xb105_mini-imagenet_5way-1shot.py 

# 测试过程(5way1shot训练为例)
python tools/classification/test.py configs/classification/matching_net/mini_imagenet/matching-net_resnet12_1xb105_mini-imagenet_5way-1shot.py --metric Recall
![image](https://github.com/hejinrong/tire_recognition_CAMN/assets/10822423/84ca1e98-3a0a-4a8f-ad48-6088595561a8)

参考代码库：
https://github.com/open-mmlab/mmfewshot

