# StocBio_hp
Codes for paper [Bilevel Optimization: Nonasymptotic Analysis and Faster Algorithms](https://arxiv.org/pdf/2010.07962.pdf).

Our hyperparameter optimization implementation is bulit on [HyperTorch](https://github.com/prolearner/hypertorch), where we propose stoc-BiO algorithm with better performance than other bilevel algorithms.
The implementation of stoc-BiO is located in two experiments [l2reg_on_twentynews.py](https://github.com/JunjieYang97/StocBio_hp/tree/master/experimental/l2reg_on_twentynews.py) and [mnist_exp.py](https://github.com/JunjieYang97/StocBio_hp/tree/master/experimental/mnist_exp.py). We will implement our stoc-BiO as a class for an independent use soon!  

Our meta-learning part is built on [learn2learn](https://github.com/learnables/learn2learn), where we show the bilevel optimizer ITD-BiO converges faster than MAML and ANIL.

In the following, we provide some experiments to demonstrate the better performance of the proposed stoc-BiO algorithm. 

We compare our algorithm with different hyperparameter baseline algorithms on newspaper dataset:
![Algorithm_Comparison](./results/test_loss_alg.png){:height="50%" width="50%"}

We compare the different batch size of our algorithm:
![Algorithm_Comparison](./results/test_loss_batch.png)

The result on MNIST dataset

![Algorithm_Comparison](./results/test_loss_mnist.png)

This repo is still under construction and any comment is welcome! 
