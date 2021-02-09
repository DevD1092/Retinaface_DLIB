# RetinaFace detector and DLIB based 68 point landmark estimator

A [PyTorch](https://pytorch.org/) implementation of [RetinaFace: Single-stage Dense Face Localisation in the Wild](https://arxiv.org/abs/1905.00641) and DLIB based landmark estimator. RetinaFace two backbones - [Mobilenet and Resnet50]. The official code of RetinaFace in Mxnet can be found [here](https://github.com/deepinsight/insightface/tree/master/RetinaFace). Original GitHub repository of RetinaFace PyTorch [https://github.com/biubug6/Pytorch_Retinaface.git]

## Installation
##### Clone and install
1. git clone https://github.ibm.com/Deval-Mehta/RetinaFace_DLIB

2. Pytorch version 1.1.0+ and torchvision 0.3.0+ are needed.

3. Codes are based on Python 3

## Testing
1. Pretrained model weights are in the directory [./weights/] - Contains the ResNet50 and MobileNet0.25 weights:
```Shell
  ./weights/
      mobilenet0.25_Final.pth
      mobilenetV1X0.25_pretrain.tar
      Resnet50_Final.pth
```

2. Running the model for testing
>> Video file as an input
```Shell
python test_widerface_dlib_video.py 
```
>> Image list as an input
```Shell
python test_widerface_dlib_images.py 
```

3. Arguments
### Default - Resnet 50 backbone and Resnet 50 weights. To change mention
```Shell
python test_widerface_dlib_video.py --network mobile0.25
```
