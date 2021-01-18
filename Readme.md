# InStereo2K: A large real dataset for stereo matching in indoor scenes

## Overview
InStereo2K [1] contains 2050 pairs of images with high accuracy disparity maps (2000 for training, 50 for testing). 
We hope it can improve the the generalization performance of deep stereo matching networks.

Wei Bao, Wei Wang, Yuhua Xu, Yulan Guo, Siyu Hong, Xiaohu Zhang. InStereo2K: A large real dataset for stereo matching in indoor scenes. SCIENCE CHINA Information Sciences. 2020.

## Data format
To keep sub-pixel accuracy, the raw floating disparity maps are magnified 100 times and rounded, finally stored in 16-bit PNG format.
So When using the dataset, divide the disparity values by 100 to get the correct scale.

The invalid disparity is set to zero. In your training process, the invalid pixels should be kicked out.
If you use resizing to enhance the dataset in disparity range, we recommend the nearest interpolation.

## Disparity Map Samples
<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/1.png"/></div>
<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/2.png"/></div>
<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/3.png"/></div>

[[More about the dataset (video)]](https://v.youku.com/v_show/id_XNDE4MjgyNTg5Ng==.html?spm=a2h0k.11417342.soresults.dtitle)

## Evaluation
The figure below is the result of iResNet [2] finetuned using our dataset and the bad2.0 error is 18.5. The bad 2.0 error of DeepPruner [3] fine-tuned using the dataset is 16.5. Note that the Middlebury training set is not used during the fine-tuning process, so it can be seen as an unseen data set. For more information, please refer to our paper.

<img width="600" src="https://github.com/YuhuaXu/StereoDataset/blob/master/samples/eva_mid.png"/></div>

## Download
1. BaiDu（百度网盘）: https://pan.baidu.com/s/160BB5bfs0oABLqwJjZzYiA 

Extraction Code: 9qwt 

2. OneDrive Link:
https://1drv.ms/u/s!AhORN5PjOtgJgQVku2DVLD8Xaqkk?e=9DTd0n

https://1drv.ms/u/s!AoQcUQo52MO6aFIMqKJKDmzCxuQ?e=D8G0zi

## Contact
For questions, please send an email to xyh_nudt@163.com

## Reference
[1] Wei Bao, Wei Wang, Yuhua Xu, Yulan Guo, Siyu Hong, Xiaohu Zhang. InStereo2K: A large real dataset for stereo matching in indoor scenes. SCIENCE CHINA Information Sciences. 2020.

[2] Z Liang, Y Guo*, Y Feng, W Chen, L Qiao, L Zhou, J Zhang, H Liu. Stereo Matching Using Multi-level Cost Volume and Multi-scale Feature Constancy. IEEE Transactions on Pattern Analysis and Machine Intelligence. 2019.

[3] Duggal S, Wang S, Ma W C, et al. DeepPruner: Learning Efficient Stereo Matching via Differentiable PatchMatch[C]//Proceedings of the IEEE International Conference on Computer Vision. 2019: 4384-4393.
