# Papers read
A list of some of the more note-worthy papers I read

### Basic research/fundamental research
- On calibration of modern neural networks - June 2017 - shows that neural networks' confidences are not always very representative of probabilities and how to get them closer to probabilities
- Group Normalization - March 2018 - activation normalization, alternative to Batch Normalization that doesn't depend on batch size and works very well
- Weight Standardization - March 2019 - weights normalization that shows that by shifting means to 0 significant gains on accuracy can be achieved
- Heated-Up Softmax Embedding - September 2018 - shows how heating up logits of softmax layer leads to better separation between embeddings for different categories

### Segmentation
- Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation - March 2018 - vastly improved results over FCN
- Spatial As Deep: Spatial CNN for Traffic Scene Understanding - December 2017 - neat idea helping segmentation of long and partially obstructed objects, e.g. lane lines

### Non-maximum suppression
- Improving Object Detection With One Line of Code - August 2017 - a smarter NMS than hard treshold


### Image ranking
- In Defense of the Triplet Loss for Person Re-Identification - November 2017 - introduces batch-hard triplet loss + soft-margin, gives tips on what metrics to monitor during training (loss isn't necessarily the most appropriate one)
