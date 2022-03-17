# Parameter Efficiency Leaderboard

## MNIST, 99% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- |
| 1,398  | Three-layer Sharpened Cosine Similarity with paired depthwise and pointwise operations  | [code](https://colab.research.google.com/drive/1Lo-P_lMbw3t2RTwpzy1p8h0uKjkCx-RB?usp=sharing) | Raphael Pisoni |


## Fashion MNIST, 90% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- |
| 7,659 | Three-layer Sharpened Cosine Similarity with 12 5x5 kernels in each layer. | [code](https://github.com/brohrer/scs_torch_gallery/blob/main/fashion_90_7659.py) | Brandon Rohrer |


## CIFAR-10, 80% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- |
| 47,643 | Three-layer Sharpened Cosine Similarity with 30 5x5 kernels in each layer. | [code](https://github.com/brohrer/scs_torch_gallery/blob/main/cifar10_80_47643.py) | Brandon Rohrer |


## CIFAR-10, 90% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- |
|  103,000 | ConvMixer-256/8 (Patches Are All You Need?), achieved 91.26%. | [paper](https://arxiv.org/pdf/2201.09792v1.pdf), [code](https://github.com/locuslab/convmixer) | Asher Trockman, J. Zico Kolter |
| 639,702 | kEffNet-B0, an EfficientNet with paired pointwise convolutions, achieved 91.64%. | [paper](https://www.researchgate.net/publication/355214501_Grouped_Pointwise_Convolutions_Significantly_Reduces_Parameters_in_EfficientNet/fulltext/6168f71b66e6b95f07cb7118/Grouped-Pointwise-Convolutions-Significantly-Reduces-Parameters-in-EfficientNet.pdf) | Joao Paulo Schwarz Schuler, Santiago Romani, Mohamed Abdel-Nasser, Hatem Rashwan, Domenec Puig |
 | 1.2M | SCS-based network achieved 91.3%. | [code](https://github.com/hukkelas/sharpened_cosine_similarity_torch/blob/main/sharpened_cosine_similarity.py) | Håkon Hukkelås |


## ImageNet top-1, 80% accuracy

| Parameters  | Model | Links | Authors |
| ------------- | ------------- |
| 21.1M | ConvMixer-768/32 (Patches Are All You Need?), achieved 80.16%. | [paper](https://arxiv.org/pdf/2201.09792v1.pdf), [code](https://github.com/locuslab/convmixer) | Asher Trockman, J. Zico Kolter |
    

## Why parameter efficiency?

There are a lot of different dimensions to a model's performance and parameter efficiency is one that gets overlooked. If two models have similar accuracy, but one has fewer parameters it will probably be cheaper to store, run, distribute, and maintain. Some model families are inherently more parameter efficient than others, but those differences aren't showcased in accuracy leaderboards. This is a chance for parameter efficient architectures to get their time in the spotlight.

## Isn't this just a cherry-picked metric that sharpened cosine similarity does well on?

Yes. 
