# RE-DGRL: Robust and Effcient Representation Learning for Discrete-time Dynamic Graph

This repository is our PyTorch implementation of RE-DGRL.

## Requirements

```shell
pip install -r requirements.txt
```

## How to run

You can run the RE-DGRL with the following commands:

```shell
# UCI
python main.py --dataset uci-msg --lr 0.01 --maml_lr 0.008 --drop_rate 0.16 --window_num 8
# DBLP
python main.py --dataset dblp --lr 0.007 --maml_lr 0.003 --drop_rate 0.09 --window_num 8
# BitcoinAlpha
python main.py --dataset bitcoinalpha --lr 0.2 --maml_lr 0.003 --drop_rate 0.1 --window_num 8
# BitcoinOTC
python main.py --dataset bitcoinotc --lr 0.003 --maml_lr 0.006 --drop_rate 0.4 --window_num 7
# Reddit-Title
python main.py --dataset reddit_title --lr 0.07 --maml_lr 0.0009 --drop_rate 0.16 --window_num 10
# stackoverflow
python main.py --dataset stackoverflow_M --lr 0.03 --maml_lr 0.001 --drop_rate 0.1 --window_num 8 --num_layers 1 --num_hidden 32 --out_dim 16

```


## Acknowledgement

Our source code and data processing are built heavily based on the code of Roland (https://github.com/snap-stanford/roland).

We modified loader.py in graphgym, and the modified one is loader.py in this project.

The data set download address is provided in the paper.
