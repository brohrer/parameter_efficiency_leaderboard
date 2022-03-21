# Parameter Efficiency Leaderboard

## MNIST, 99% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
| 910 | ConvNet with customized Hough voting layer | [code](https://colab.research.google.com/drive/1HFwUZQ91CKMGU63KHgvS9kFZgL-w2Cya) | Satoshi Tanaka |

| 1,398  | Three-layer Sharpened Cosine Similarity with paired depthwise and pointwise operations.  | [code](https://colab.research.google.com/drive/1Lo-P_lMbw3t2RTwpzy1p8h0uKjkCx-RB?usp=sharing) | Raphael Pisoni |

## Fashion MNIST, 90% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
| 1,890 | ConvNet with customized Hough voting layer | [code](https://colab.research.google.com/drive/1Jl5OZFTINXkJPPJ5-Xe3_1uV4iAIzqwt) | Satoshi Tanaka |
| 3,423 | Four-layer SCSMixer (layers include depthwise and pointwise operations) with 26 3 x 3 kernels in each layer | [code](https://github.com/brohrer/scs_torch_gallery/blob/main/fashion_90_3423.py) | Brandon Rohrer |
| 7,156  | WaveMix Lite-8/5.  | [code](https://github.com/pranavphoenix/WaveMix), [paper](https://arxiv.org/pdf/2203.03689.pdf) | Pranav Jeevan P, Amit Sethi|
| 7,659 | Three-layer Sharpened Cosine Similarity with 12 5x5 kernels in each layer. | [code](https://github.com/brohrer/scs_torch_gallery/blob/main/fashion_90_7659.py) | Brandon Rohrer |

## Fashion MNIST, 95% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |


## CIFAR-10, 80% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
| 45,962  | WaveMix Lite-32/4 (ff=16, mult=1, dropout=0.25).  | [code](https://github.com/pranavphoenix/WaveMix), [paper](https://arxiv.org/pdf/2203.03689.pdf) | Pranav Jeevan P, Amit Sethi|
| 47,643 | Three-layer Sharpened Cosine Similarity with 30 5x5 kernels in each layer. | [code](https://github.com/brohrer/scs_torch_gallery/blob/main/cifar10_80_47643.py) | Brandon Rohrer |


## CIFAR-10, 90% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
|  103,000 | ConvMixer-128/4, achieved 91.26%. | [paper](https://arxiv.org/pdf/2201.09792v1.pdf), [code](https://github.com/locuslab/convmixer) | Asher Trockman, J. Zico Kolter |
| 639,702 | kEffNet-B0, an EfficientNet with paired pointwise convolutions, achieved 91.64%. | [paper](https://www.researchgate.net/publication/355214501_Grouped_Pointwise_Convolutions_Significantly_Reduces_Parameters_in_EfficientNet/fulltext/6168f71b66e6b95f07cb7118/Grouped-Pointwise-Convolutions-Significantly-Reduces-Parameters-in-EfficientNet.pdf) | Joao Paulo Schwarz Schuler, Santiago Romani, Mohamed Abdel-Nasser, Hatem Rashwan, Domenec Puig |
 | 1.2M | SCS-based network achieved 91.3%. | [code](https://github.com/hukkelas/sharpened_cosine_similarity_torch/blob/main/sharpened_cosine_similarity.py) | Håkon Hukkelås |

## CIFAR-10, 95% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
|  594,000 | ConvMixer-256/8 | [paper](https://arxiv.org/pdf/2201.09792v1.pdf), [code](https://github.com/locuslab/convmixer) | Asher Trockman, J. Zico Kolter |


## ImageNet top-1, 80% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
| 21.1M | ConvMixer-768/32 | [paper](https://arxiv.org/pdf/2201.09792v1.pdf), [code](https://github.com/locuslab/convmixer) | Asher Trockman, J. Zico Kolter |

## ImageNet top-1, 90% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- | ------------- | ------------- |
| 390M | EfficientNet-B6-Wide with Meta-Pseudo Labels with 300M unlabled images from [JFT](https://paperswithcode.com/dataset/jft-300m)| [paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Pham_Meta_Pseudo_Labels_CVPR_2021_paper.pdf), [code](https://github.com/google-research/google-research/tree/master/meta_pseudo_labels) | Hieu Pham, Zihang Dai, Qizhe Xie, Quoc V. Le |



## Why parameter efficiency?

There are a lot of different dimensions to a model's performance and parameter efficiency is one that gets overlooked. If two models have similar accuracy, but one has fewer parameters it will probably be cheaper to store, run, distribute, and maintain. Some model families are inherently more parameter efficient than others, but those differences aren't showcased in accuracy leaderboards. This is a chance for parameter efficient architectures to get their time in the spotlight.

## Isn't this just a cherry-picked metric that sharpened cosine similarity does well on?

Yes. 
