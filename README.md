![image](https://github.com/Pollycarpus/frcnn-from-scratch-with-keras/blob/master/Picture1.jpg)
![image](https://github.com/Pollycarpus/frcnn-from-scratch-with-keras/blob/master/Picture2.jpg)

# Traffic Sign Detection Using CNN for Indonesia
-- under Apache 2.0 license --

- **Simple faster-RCNN codes in Keras!**

- **RPN (region proposal layer) can be trained separately!**

- **VGG16**

- **ResNet50**

- **eval added!**


## Frameworks
Tested with Tensorflow==1.12.0 and Keras 2.2.4.

## trained model
[1] frcnn-vgg16

https://drive.google.com/file/d/1AjgMEb2DJSjCqJSAO8hMntout0m9Ccbo/view?usp=sharing

[1] config.pickle:

https://drive.google.com/file/d/10iSDUjRRQWW2ptQq5DETlV9n_aQ59vag/view?usp=sharing

[2] frcnn-resnet50

https://drive.google.com/file/d/1cXyQaePyU_pdVjR6k8eIXmil1Pm3WBaH/view?usp=sharing

[2] config.pickle

https://drive.google.com/file/d/1Dt1SYWO7DLxSaWYBNSC520Q4QSxV_QD0/view?usp=sharing

## Download pretrained weights.
Using imagenet pretrained VGG16 weights will significantly speed up training.

Download and place it in the root directory.

You can choose other base models as well.

```
# place weights in pretrain dir.
mkdir pretrain & mv pretrain

# download models you would like to use.
# for VGG16
wget https://github.com/fchollet/deep-learning-models/releases/download/v0.1/vgg16_weights_tf_dim_ordering_tf_kernels.h5

# for resnet 50
wget https://github.com/fchollet/deep-learning-models/releases/download/v0.1/resnet50_weights_tf_dim_ordering_tf_kernels.h5
```

Other tensorflow pretrained models are in bellow.

https://github.com/fchollet/deep-learning-models/releases/

## Future works
YOLO will be added soon!

# Dataset setup.

Simply provide a text file, with each line containing:
```
filepath,x1,y1,x2,y2,class_name
```
For example:
```dataset.txt
/data/imgs/img_001.jpg,837,346,981,456,cow /data/imgs/img_002.jpg,215,312,279,391,cat
```
# Instructions

First upload .ipynb files to notebook

To train model: run train_model.ipynb

To test model: run test_model.ipynb

To test model on video: run test_on_video.ipynb

# Author
Pollycarpus
