## TireNet —— A method for tire track image recognition
![image](https://github.com/user-attachments/assets/ea532797-e853-4d57-8afb-c8550205ce4c)

## Environment requirements
matplotlib==3.7.4
matplotlib-inline==0.1.6
mdurl==0.1.2
mmcls==0.23.0
mmcv-full==1.5.2
mmdet==2.24.1
numpy==1.24.4

## Training process (Example for 5-way 1-shot training)
python tools/classification/train.py configs/classification/matching_net/mini_imagenet/matching-net_resnet12_1xb105_mini-imagenet_5way-1shot.py 

## Testing process (Example for 5-way 1-shot testing)
python tools/classification/test.py configs/classification/matching_net/mini_imagenet/matching-net_resnet12_1xb105_mini-imagenet_5way-1shot.py --metric Recall

### Reference code repository and install environment method(Special thanks to the OpenMMLab community for their contributions):
https://github.com/open-mmlab/mmfewshot
https://mmfewshot.readthedocs.io/en/latest/

### Access to the self-built dataset:
https://drive.google.com/file/d/18hlR5eiQnt266jZVnR1PEgrScwLHogsJ/view?usp=drive_link


