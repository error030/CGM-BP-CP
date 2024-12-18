# We are speeding up the code cleanup and the code will be made public soon！！！
# Long-Tailed Classification by Efficient Contrast Learning with High Quality and High Relevance Latent Features 
Python code for paper entitled "Long-Tailed Classification by Efficient Contrast Learning with High Quality and High Relevance Latent Features"

#### Description:
It is important to learn robust feature representations from long-tail distributed data. Recently, contrast learning has made remarkable achievements in long-tail learning, Contrastive learning can be seen as optimizing the lower bound of mutual information, but previous methods made inaccurate assumptions about model distribution and ignored the long tail problem of sample space, resulting in the lower bound not being tight enough. Besides, previous contrast learning methods made insufficient use of information to guide feature representation learning. In this paper, we first propose a loss function using batch sample features and class prototypes to construct a Conditional Gaussian mixture distribution (CGM-BF-CP), and prove its generalization ability from the perspective of generalization error upper bound. Then we create High Quality and High Relevance KNN graph to model relation between features and proposed a corresponding loss function, Graph based Contrast Learning Loss (GCLL). The feature information can be transferred between classes through this graph, so that the tail class features can be better learned. The experimental results on Cifar10/100-LT and ImageNet-LT show that our proposed model is competitive with the latest methods.

#### Requirements:
*    Python 3.10.12
*    Pytorch 2.0.0+cpu
*    tqdm
*    tensorboard_logger-0.1.0
*    matplotlib


#### Long-tailed recognition accuracy:
Dataset | Backbone | Epochs | Top-1 Acc(%)
---- | :----: | :----: | :----: 
CIFAR-100-LT (IF = 100) | ResNet-32 | 200 | 52.4
CIFAR-100-LT (IF = 50) | ResNet-32 | 200 | 56.6
CIFAR-10-LT (IF = 100) | ResNet-32 | 200 | 85.6
CIFAR-10-LT (IF = 50) | ResNet-32 | 200 | 88.0
ImageNet-LT（TF=256）| ResNext-50 | 90 | 57.1
