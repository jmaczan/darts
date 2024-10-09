# Lightning Differentiable Architecture Search

> A modern PyTorch Lightning reimplementation of Differentiable Architecture Search

This project is a fork of the original [DARTS repository](https://github.com/quark0/darts). The goal is to enable further research and development in a field of Neural Architecture Search, through a gradual upgrade and improvement of the original Differentiable Architecture Search implementation

The modifications include:

- Upgrading code to PyTorch 2.x
- Rewriting the code to use PyTorch Lightning for training and architecture search
- Make things optimized for modern hardware
- Fix bugs

The scope is now limited to Convolutional Neural Networks (CNN) and once the reimplementation is done, I will expand it to other kinds of neural nets

The original paper:

> [DARTS: Differentiable Architecture Search](https://arxiv.org/abs/1806.09055)\
> Hanxiao Liu, Karen Simonyan, Yiming Yang.\
> _arXiv:1806.09055_.

<p align="center">
  <img src="img/darts.png" alt="darts" width="48%">
</p>

The algorithm is based on continuous relaxation and gradient descent in the architecture space. It is able to efficiently design high-performance convolutional architectures for image classification (on CIFAR-10 and ImageNet) and recurrent architectures for language modeling (on Penn Treebank and WikiText-2). Only a single GPU is required.

## Requirements

- Python >= 3.10
- PyTorch >= 2.4.1
- PyTorch Lightning >= 2.4.0

## Cite

If you use this project in your research, please use the following citation:

```bibtex
@misc{Maczan_DARTS_2024,
  title = "Lightning Differentiable Architecture Search: A modern PyTorch Lightning reimplementation of Differentiable Architecture Search (DARTS)",
  author = "{Maczan, Jędrzej Paweł}",
  howpublished = "\url{https://github.com/jmaczan/darts}",
  year = 2024,
  publisher = {GitHub}
}
```

Please strongly consider to cite the original [DARTS paper](https://arxiv.org/abs/1806.09055) as well:

```bibtex
@article{liu2018darts,
  title={DARTS: Differentiable Architecture Search},
  author={Liu, Hanxiao and Simonyan, Karen and Yang, Yiming},
  journal={arXiv preprint arXiv:1806.09055},
  year={2018}
}
```

## License

Apache License 2.0

## Authors

Original DARTS paper and implementation: Hanxiao Liu, Karen Simonyan, Yiming Yang

Lightning Differentiable Architecture Search: Jędrzej Maczan
