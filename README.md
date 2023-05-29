# Parallel Knowledge Enhancement based Framework for Multi-behavior Recommendation

This repository contains TensorFlow codes and datasets for the paper.

## Environment
The codes of PKEF are implemented and tested under the following development environment:
* python=3.6.13
* tensorflow=1.15.0
* numpy=1.19.2
* scipy=1.5.2

## Datasets
We utilized three datasets to evaluate PKEF: <i>Beibei, Taobao, </i>and <i>Tmall Contest</i>. The <i>purchase</i> behavior is taken as the target behavior for all datasets. The last target behavior for the test users are left out to compose the testing set. We filtered out users and items with too few interactions.

## Just Run It！

* Beibei
```
python PKEF_final.py --data beibei
```
* Taobao
```
python PKEF_final.py --data taobao
```
* Tmall
```
python PKEF_final.py --data tmall --gnn_layer "[4, 1, 1, 1]" --coefficient "[0.0/6, 4.0/6, 0.0/6, 2.0/6]"
```
