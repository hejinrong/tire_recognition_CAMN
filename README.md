# tire_recognition_CAMN

# 环境要求
matplotlib==3.7.4
matplotlib-inline==0.1.6
mdurl==0.1.2
mmcls==0.23.0
mmcv-full==1.5.2
mmdet==2.24.1
numpy==1.24.4
# 命令行搭建环境
# 创建环境
conda create -n tire python=3.7 -y
conda activate tire
# 安装基础环境
pip install -r requirement.txt #安装基础环境
# 搭建环境
cd tire_recognition_CAMN
pip install -r requirements/build.txt
pip install -v -e .  # or "python setup.py develop"

参考代码库：
https://mmfewshot.readthedocs.io/en/latest/install.html
https://github.com/open-mmlab/mmfewshot

