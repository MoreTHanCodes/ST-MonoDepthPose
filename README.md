# Leveraging the Spatio-Temporal Structure of Image Sequences for Self-Supervised Monocular Depth-Pose Learning
<p align="center">
    <b>Tao Han<sup>1</sup>, Tingxiang Fan<sup>2</sup> and Jia Pan<sup>2</sup>
</p>
<p align="center">
    <b><a href="https://www.cityu.edu.hk/">City University of Hong Kong<sup>1</sup></a>, <a href="https://www.hku.hk/">The University of Hong Kong<sup>2</sup></a></b>
</p>

## Abstract

Most existing methods in self-supervised depth-pose learning have not fully explored the underlying spatio-temporal structure of video input, which limits their performance in both accuracy and generalization. In this work, we consider the issue from two aspects: i) the temporal connection between sequential images should be perceived and utilized by the models in inference stage, and ii) the multiple-view geometry between sequential images is essential for the estimation task which is unnecessary to be learned from scratch. To tackle the problem, we propose a novel system that can leverage the spatio-temporal structure of image sequences for the task. Specifically, we design a unified recurrent network architecture to capture temporal information in video data and extract reliable features for more accurate estimations. Secondly, we replace the widely used learn-from-scratch inferring framework with a geometry-aided framework, where network models focus on depth and optical flow learning and a two-view geometry module is employed for pose recovery and depth-pose scale alignment to boost system generalization. Thirdly, we introduce the technique of per-pixel reprojection loss into the geometry-aided framework to further improve system performance based on self-supervised training. Extensive experiments show that the proposed system not only reaches state-of-the-art performance on KITTI depth and pose estimation but also demonstrates its advantage in terms of generalization ability.

<p align="center">
    <img src="figs/fig_overview.pdf" width="640" />
</p><p align="center">
    <i>Figure 1. System overview. All system modules work online during training and inference. Please refer to our paper for more details about our system.</i>
</p>
