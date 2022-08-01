# Graduation-thesis-project
Graduation-thesis-project

# Relational Embedding for Few-Shot Classification

## Abstract

The success of various models of deep learning depends on a large number of training samples. However, in reality, the acquisition of data samples requires a large amount of human and material costs, which makes it impossible to obtain a large number of training samples. Due to the difficulty of obtaining a large amount of data, the concept of few-shot learning is put forward, which can achieve good results in the case of few samples. Therefore, few-shot learning has become the focus of people's attention, this thesis will focus on few-shot learning as the research object.
In this thesis, firstly, a garbage classification dataset of 47951 images is constructed, which contains 117 categories, and the number of each category ranges from 208 to 1150 images. Secondly, based on Relational Embedding for Few-Shot Classification(ReNet) ，This thesis will reproduce the model. On the basis of reproduction, two types of exploration are carried out: 1. Resnet-12 residual network exploration with introduction of LSA and BotNet module, the maximum improvement in CUB bird dataset is 0.17%. 2. Data augmentation and Snapshot Ensemble exploration with introduction of MixUp、CutMix、Radom Erasing、Trivial Augment and so on, the CUB and CIFAR_FS public datasets and self-made garbage classification datasets have improved by 4.1% and 2.4% in 1/5-shot settings , and SOTA has been achieved in CUB and CIFAR_FS public datasets. Thirdly, the ViT, T2T, Distil-T2T and CCT models are reproduced in this thesis as the few-shot backbone model. Based on reproduction, Res9ViT and its derived model are proposed. The performance of the model is better than ViT by 26% and 23% in 1/5-shot setting. Finally, ViT model and the Res9ViT model proposed in this thesis are applied to ReNet, and the CUB and garbage classification datasets are significantly improved by 1.8% and 1.2%.

#### Key Words：Few Shot Learning; Self-built Dataset; Data Augmentation; Residual Network; Vision Transformer

## some highlight content
### 1.data augmentation && Snapshot ensembles
#### data augmentation:Overall flow chart of thought
Methods of data augmentation adopted in training:MixUp,CutMix,RandomErasing,TrivialAugment

Methods of data augmentation adopted in testing: Horizon Flip,CenterCrop, RandomCrop

<img src="https://github.com/yangtiming/Graduation-thesis-project/blob/master/imgs/g-1.jpeg" width="700px">

#### Snapshot ensembles

The weights of data augmentation are used in Snapshot ensembles

<img src="https://github.com/yangtiming/Graduation-thesis-project/blob/master/imgs/g-2.jpeg" width="700px">

#### results

<img src="https://github.com/yangtiming/Graduation-thesis-project/blob/master/imgs/g-3.jpeg" width="400px">

### 2.data augmentation && Snapshot ensembles





