# 系统与计算神经科学作业

本项目是基于RSNN的模拟小鼠决策任务的程序。程序模拟了小鼠的感知、工作记忆和决策实验。实验设定小鼠在丁字形通道内，先经过带有提示信息的通道，再经过没有信息的通道，最终路口处决定左转或右转。通过奖励信息对小鼠行为进行训练。本程序通过计算建模对此实验进行模拟。搭建RSNN循环脉冲神经网络模拟小鼠大脑活动，通过监督训练模拟小鼠的学习行为，最终使得网络具有感知、工作记忆和决策能力。



## Requirements

- Python >=3.7.10,<3.10

## Setting things up

## Using Pip
To install the most recent stable release from the GitHub repository

```
pip install git+https://github.com/BindsNET/bindsnet.git
```

## Getting started

To run a near-replication of the SNN from [this paper](https://www.frontiersin.org/articles/10.3389/fncom.2015.00099/full#), issue

```
cd examples/mnist
python eth_mnist.py
```

There are a number of optional command-line arguments which can be passed in, including `--plot` (displays useful monitoring figures)
## Running the tests

Issue the following to run the tests:

```
python -m pytest test/
```

Some tests will fail if Open AI `gym` is not installed on your machine.


## Result

<p align="middle">
<img src="data/task2/result" alt="BindsNET%20Benchmark"  width="503" height="403">
</p>

All simulations run on Ubuntu 16.04 LTS with Intel(R) Xeon(R) CPU E5-2687W v3 @ 3.10GHz, 128Gb RAM @ 2133MHz, and two GeForce GTX TITAN X (GM200) GPUs. Python 3.6 is used in all cases. Clock time was recorded for each simulation run. 



## Contributors

- Daniel Saunders ([email](mailto:djsaunde@cs.umass.edu))
