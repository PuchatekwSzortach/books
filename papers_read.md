# Papers read
A list of some of the more note-worthy papers I read

### Basic research/fundamental research
- On calibration of modern neural networks - June 2017 - shows that neural networks' confidences are not always very representative of probabilities and how to get them closer to probabilities
- Group Normalization - March 2018 - activation normalization, alternative to Batch Normalization that doesn't depend on batch size and works very well
- Weight Standardization - March 2019 - weights normalization that shows that by shifting means to 0 significant gains on accuracy can be achieved
- Heated-Up Softmax Embedding - September 2018 - shows how heating up logits of softmax layer leads to better separation between embeddings for different categories

### Segmentation
- Fully Convolutional Networks for Semantic Segmentation - November 2013 - explains how convolutional networks and fully connected networks can be translated into each other, shows how to perform segmentations with convolutional layers only
- Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation - March 2018 - vastly improved results over FCN
- Spatial As Deep: Spatial CNN for Traffic Scene Understanding - December 2017 - neat idea helping segmentation of long and partially obstructed objects, e.g. lane lines
- Mask R-CNN - January 2018 - explains how instance segmentation is done from regions proposals, and how human pose estimation can be treated as a category segmentation problem
- Simple Copy-Paste is a Strong Data Augmentation Method for Instance Segmentation - June 2021 - shows that pasting instances on backgrounds of other images creates useful additional data for segmentation tasks

### Non-maximum suppression
- Improving Object Detection With One Line of Code - August 2017 - a smarter NMS than hard treshold

### Image ranking
- In Defense of the Triplet Loss for Person Re-Identification - November 2017 - introduces batch-hard triplet loss + soft-margin, gives tips on what metrics to monitor during training (loss isn't necessarily the most appropriate one)
- Hard-Aware Point-to-Set Deep Metric for Person Re-identification - July 2018 - introduces point to set loss that is a generalization of BatchHard loss from `In Defense of the Triplet Loss for Person Re-Identification`. Loss is made from a weighted sum of all positive and negative samples with respect to anchor imge. Improves results and is more resilient to outliers/mislabeled samples.
- Combination of Multiple Global Descriptors for Image Retrieval - March 2019 - image ranking model based on a combination of fixed features build on top of convolutional channels.

### Generative adversarial networks
- Image-to-Image Translation with Conditional Adversarial Networks - November 2016 - also know as pix2pix - introduces patch-wise discriminator. Discriminator predicts on 70x70 patches instead of entire image. Gives reasonable ok results for 256x256 images in image-to-image translation tasks that don't require large changes in shape.
- - Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks - March 2017 - also known as CycleGAN - shows a method to train generator mapping images from distribution X to distribution Y without paired inputs x -> y.
- AutoRetouch: Automatic Professional Face Retouching - January 2021 - introduces a GAN model for automatic skin retouching and skin retouching dataset (FFHQR)
