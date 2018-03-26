# XDYangLiu.github.io
Codes for paper "Global Temporal Representation based CNNs for Infrared Action Recognition"
### Abstract
Infrared human action recognition has many advantages, i.e. it is insensitive to illumination change, appearance variability and shadows. Existing methods for infrared action recognition are either based on spatial or local temporal information, however, the global temporal information, which can better describe the movements of body parts across the whole video, is not considered. In this letter, we propose a novel global temporal representation named Optical-Flow Stacked Difference Image (OFSDI) and extract robust and discriminative feature from infrared action data by considering the local, global, and spatial temporal information together. Due to the small size of infrared action dataset, we first apply CNN on local, spatial, and global temporal stream respectively to obtain efficient convolutional feature maps from the raw data rather than train a classifier directly. Then these convolutional feature maps are aggregated into effective descriptors named three-stream trajectory-pooled deep-convolutional descriptors (TSTDDs) by trajectory-constrained pooling. Furthermore, we improve the robustness of these features by using Locality-constrained Linear Coding (LLC) method. With these features, a linear SVM is adopted to classify the action data in our scheme. We conduct experiments on infrared action recognition dataset InfAR and NTU RGB+D. Experimental results show that the proposed approach outperforms the representative state-of-the-art handcrafted features and deep learning features based methods for infrared action recognition.

### Model
![Image](Fig1.jpg)
Frameworks of our infrared action recognition method and the conventional method. Compared with the conventional method, our method is different in network input, CNNs structure, feature extraction, and classification strategy.

### Data
Dataset can be downloaded [here](https://drive.google.com/open?id=0B2TeCRG1hB55eGV1V2FJb19Cd2s), or [here](http://dwz.cn/61ckOm). Total in size = 7.43G. 
Data was caputred 29frames/s. During training, frames are sampled 30 frames/s. Thus, 1 image ~= 1s. 

For data argumentation and labelling, please check Section 4.4 in our paper. 
`L.Ran, Y. Zhang, Q. Zhang, T. Yang, Convolutional Neural Network Based Robot Navigation Using Uncalibrated Spherical Images, 2017.`

For more information about the formatted images and labels, please contact us at ![gmail](gmail.png) 

### Code
Source code avaliable: [navi.zip](https://github.com/hijeffery/PanoNavi/blob/master/navi.zip).
If you find the work helpful, please kindly consider to cite our paper by:
```
@article{ran2017convolutional,
  title={Convolutional Neural Network-Based Robot Navigation Using Uncalibrated Spherical Images},
  author={Ran, Lingyan and Zhang, Yanning and Zhang, Qilin and Yang, Tao},
  journal={Sensors},
  volume={17},
  number={6},
  pages={1341},
  year={2017},
  publisher={Multidisciplinary Digital Publishing Institute}
}
```

### Performance
[![Video](frontpage.png)](https://youtu.be/4ZjnVOa8cKA) [Demo](https://youtu.be/4ZjnVOa8cKA) video for navigation within campus.
Demo video is made with 15fps, ~= 15x faster than the original video.

### Reference
1. Ran, L.; Zhang, Y.; Yang, T.; Zhang, P. Autonomous Wheeled Robot Navigation with Uncalibrated Spherical Images. Chinese Conference on Intelligent Visual Surveillance. Springer, Singapore, 2016, pp. 47–55.
2. Giusti, A.; Guzzi, J.; Ciresan, D.; He, F.L.; Rodriguez, J.P.; Fontana, F.; Faessler, M.; Forster, C.; Schmidhuber, J.; Di Caro, G.; Scaramuzza, D.; Gambardella, L. A Machine Learning Approach to Visual Perception of Forest Trails for Mobile Robots. IEEE Robotics and Automation Letters 2016. 
