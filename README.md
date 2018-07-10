## PyTorch Code for 'Deep k-Means: Re-Training and Parameter Sharing with Harder Cluster Assignments for Compressing Deep Convolutions'

## Introduction

PyTorch Implementation of our ICML 2018 paper ["Deep k-Means: Re-Training and Parameter Sharing with Harder Cluster Assignments for Compressing Deep Convolutions"](https://arxiv.org/abs/1806.09228).

In our paper, we proposed a simple yet effective scheme for compressing convolutions though applying k-means clustering on the weights, compression is achieved through weight-sharing, by only recording K cluster centers and weight assignment indexes.

We then introduced a novel spectrally relaxed k-means regularization, which tends to make hard assignments of convolutional layer weights to K learned cluster centers during re-training. 

We additionally propose an improved set of metrics to estimate energy consumption of CNN hardware implementations, whose estimation results are verified to be consistent with previously proposed energy estimation tool extrapolated from actual hardware measurements.

We finally evaluated Deep k-Means across several CNN models in terms of both compression ratio and energy consumption reduction, observing promising results without incurring accuracy loss.

### PyTorch Model

- [x] Wide ResNet
- [ ] LeNet-Caffe-5

## Dependencies

Python 3.5
* [PyTorch 0.3.1](https://pytorch.org/previous-versions/)
* [libKMCUDA 6.2.1](https://github.com/src-d/kmcuda)
* sklearn 0.19.1
* matplotlib 2.2.2


## Testing Deep k-Means

* Wide ResNet

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; python WideResNet_Deploy.py

## Filters Visualization

## Citation

If you find this code useful, please cite the following paper:

    @article{deepkmeans,
        title={Deep k-Means: Re-Training and Parameter Sharing with Harder Cluster Assignments for Compressing Deep Convolutions},
        author={Junru Wu, Yue Wang, Zhenyu Wu, Zhangyang Wang, Ashok Veeraraghavan, Yingyan Lin},
        journal={ICML},
        year={2018}
    }
