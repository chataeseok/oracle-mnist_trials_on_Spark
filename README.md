# Oracle-MNIST trial on Spark

[![Readme-JA](https://img.shields.io/badge/README-Japanese-red.svg)](README.ja.md)

This is an expandable trial based on the `Oracle-MNIST` dataset, using the `Spark` distributed computing framework. In this experiment, a `LeNet-5` neural network was trained.

## Original paper:
A dataset of oracle characters for benchmarking machine learning algorithms. Mei Wang, Weihong Deng. 
[Scientific Data](https://www.nature.com/articles/s41597-024-02933-w)

## Original repository: 
[https://github.com/wm-bupt/oracle-mnist](https://github.com/wm-bupt/oracle-mnist)

## Usage:
```bash
spark-submit training.py \
# custom source assignment, for example,
--master <your Spark standalone url> \
--total-executor-cores 4 \
--executor-cores 1 \
--executor-memory 2G \
--driver-memory 4G \
```

I would like to express my sincere gratitude to the original authors.