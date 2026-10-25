# Deep Learning (NYU, Spring 2021)

Homeworks and the final project for Deep Learning, NYU Spring 2021.

Class materials: https://github.com/Atcold/NYU-DLSP21

## Contents

| Folder | Topic |
| --- | --- |
| [`hw1`](hw1/) | Backpropagation theory (`theory.tex`) and an MLP implemented from scratch (`mlp.py`) |
| [`hw2`](hw2/) | Convolutional neural nets (cats vs. dogs) and recurrent neural nets (echo / variable-delay tasks) |
| [`hw3`](hw3/) | Energy-based models and structured prediction (handwritten word recognition, optimal path finding) |
| [`final`](final/) | Semi-supervised image classification with MoCo (team project) |

## Final project

The task was image classification over 800 classes, with 25,600 labeled training images, 25,600 labeled validation images and 512,000 unlabeled images.

We used [MoCo](https://github.com/facebookresearch/moco) as our self-supervised pretraining framework and combined it with design choices from other models. Most of the code is based on the MoCo reference implementation.

We reached **30.48% accuracy** with 250 epochs of pretraining, then 100 epochs training a classifier on frozen features, then 100 epochs fine-tuning with unfrozen features.

- `final/dl05/`: training and evaluation code, plus Slurm `sbatch` scripts
- `final/log/`: training logs
- `final/addition/`: label-request files for the additional labeled data round
