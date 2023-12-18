# We-Know-Who-Win

This repository contains the Pytorch implementation code for the paper "We Know Who Wins: Graph-oriented Approaches of Passing Networks for Predictive Football Match Outcomes"

## Architectures
---

<p align="center">
![Model_Structure](model_structure.png)
</p>

Both the passing graph and in-game features of each team are input to the model. The passing graph passes through three convolution blocks consisting of graph convolution-dropout-elu layer to be pooled into graph embedding. The graph embeddings of both teams that have been fused with the in-game features are combined again to finally return the probability for each class.
