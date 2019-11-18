# InStereo2K: A large real dataset for stereo matching in indoor scenes

## Overview
It contains 2050 pairs of images with high accuracy disparity maps (2000 for training, 50 for testing). 
We hope it can improve the the generalization performance of deep stereo matching networks.

## Data format
To keep sub-pixel accuracy, the raw floating disparity maps are magnified 100 times and rounded, finally stored in 16-bit PNG format.
So When using the dataset, divide the disparity values by 100 to get the correct scale.

The invalid disparity is set to zero. In your training process, the invalid pixels should be kicked out.
If you use resizing to enhance the dataset in disparity range, we recommend the nearest interpolation.

## Dispartiy Map Samples
<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/1.png"/></div>
<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/2.png"/></div>
<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/3.png"/></div>

[[More about the dataset (video)]](https://v.youku.com/v_show/id_XNDE4MjgyNTg5Ng==.html?spm=a2h0k.11417342.soresults.dtitle)

##Evaluation

## Download
https://pan.baidu.com/s/160BB5bfs0oABLqwJjZzYiA 

Extraction Code: 9qwt 

## Contact
For questions, please send an email to xyh_nudt@163.com
