# VS-Graph: Scalable and Efficient Graph Classification Using Hyperdimensional Computing

Official implementation for the paper: [**"VS-Graph: Scalable and Efficient Graph Classification Using Hyperdimensional Computing"**](https://arxiv.org/abs/2512.03394)


## 1. Overview
VS-Graph is a novel vector-symbolic graph learning framework designed to bridge the gap between the computational efficiency of Hyperdimensional Computing (HDC) and the structural expressiveness of Message Passing Graph Neural Networks (GNNs).

### Key Components:
- **Spike Diffusion:** A lightweight mechanism that propagates "spikes" through the graph to compute topology-derived node signatures and ordinal rankings.

- **Associative Message Passing:** A multi-hop neighborhood aggregation scheme using idempotence-based logical operators (OR) to refine representations entirely within the hypervector space.

- **Graph-Level Readout:** An element-wise mean operation that produces fixed $D$-dimensional graph embeddings for prototype-based classification.


The provided Jupyter Notebook contains the full pipeline for reproducing results on TUDataset benchmarks.

### Requirements
The implementation uses **DGL (Deep Graph Library)** and **PyTorch**.

### Configuration

You can modify the Quick config section in the code to test different settings:

`DATASET`: Benchmarks include MUTAG, PTC_FM, PROTEINS, DD, and NCI1.

`FEAT_TYPE`: Supports hd_binary (default), hd_bipolar, or onehot.

`D_HD`: Hypervector dimensionality.

`ALPHA`: Residual blend factor for the convex combination of node states

### Citation

```bibtex
@article{poursiami2025vsgraph,
  title   = {VS-Graph: Scalable and Efficient Graph Classification Using Hyperdimensional Computing},
  author  = {Poursiami, Hamed and Snyder, Shay and Cong, Guojing and Potok, Thomas and Parsa, Maryam},
  journal = {arXiv preprint arXiv:2512.03394},
  year    = {2025}
}
