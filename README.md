# A Coding Framework and Benchmark towards Low-Bitrate Video Understanding (TPAMI2024)

PyTorch Implementation of our paper:

> **A Coding Framework and Benchmark towards Low-Bitrate Video Understanding**
>
> Yuan Tian; Guo Lu; Yichao Yan; Guangtao Zhai; Li Chen; Zhiyong Gao
> [[IEEE Explore](https://ieeexplore.ieee.org/abstract/document/10440520/)]
> [[ArXiv](https://arxiv.org/abs/2202.02813)]



## Main Contribution
Video compression is indispensable to most video analysis systems. Despite saving transportation bandwidth, it also deteriorates downstream video understanding tasks, especially at low-bitrate settings. To systematically investigate this problem, we first thoroughly review the previous methods, revealing that three principles, i.e., **task-decoupled, label-free, and data-emerged semantic prior**, are critical to a machine-friendly coding framework but are not fully satisfied so far. In this paper, we propose a traditional-neural mixed coding framework that simultaneously fulfills all these principles, by taking advantage of both traditional codecs and neural networks (NNs). On one hand, the traditional codecs can efficiently encode the pixel signal of videos but may distort the semantic information. On the other hand, highly non-linear NNs are proficient in condensing video semantics into a compact representation. The framework is optimized by ensuring that a transportation-efficient semantic representation of the video is preserved w.r.t. the coding procedure, which is spontaneously learned from unlabeled data in a self-supervised manner. The videos collaboratively decoded from two streams (codec and NN) are of rich semantics, as well as visually photo-realistic, empirically boosting several mainstream downstream video analysis task performances without any post-adaptation procedure. Furthermore, by introducing the attention mechanism and adaptive modeling scheme, the video semantic modeling ability of our approach is further enhanced. Finally, we build a low-bitrate video understanding benchmark with three downstream tasks on eight datasets, demonstrating the notable superiority of our approach. 


## Guidance
The codes and models are still being re-organized. 
However, its evaluation protocol and downstream task models are available at [SMC](https://github.com/tianyuan168326/VideoSemanticCompression-Pytorch). You can test your approach with the SMC codebase, for a fair comparison with our approaches.


## Other Info

<!-- ### References

This repository is built upon the following projects.

- [TSM](https://github.com/mit-han-lab/temporal-shift-module)
- [MMaction2](https://github.com/open-mmlab/mmaction2)
- [XMem](https://github.com/hkchengrex/XMem) -->

### Citation

Please **[★star]** this repo and **[cite]** the following video semantic compression papers if you feel our project and codes useful to your research:

```
@article{tian2024coding,
  title={A coding framework and benchmark towards low-bitrate video understanding},
  author={Tian, Yuan and Lu, Guo and Yan, Yichao and Zhai, Guangtao and Chen, Li and Gao, Zhiyong},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year={2024},
  publisher={IEEE}
}

@inproceedings{tian2023non,
  title={Non-Semantics Suppressed Mask Learning for Unsupervised Video Semantic Compression},
  author={Tian, Yuan and Lu, Guo and Zhai, Guangtao and Gao, Zhiyong},
  booktitle={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  pages={13610--13622},
  year={2023}
}

@article{tian2024smc++,
  title={SMC++: Masked Learning of Unsupervised Video Semantic Compression},
  author={Tian, Yuan and Lu, Guo and Zhai, Guangtao},
  journal={arXiv preprint arXiv:2406.04765},
  year={2024}
}

@article{tian2024free,
  title={Free-VSC: Free Semantics from Visual Foundation Models for Unsupervised Video Semantic Compression},
  author={Tian, Yuan and Lu, Guo and Zhai, Guangtao},
  journal={arXiv preprint arXiv:2409.11718},
  year={2024}
}
```


### Contact

For any questions, please feel free to open an issue or contact:

```
Yuan Tian: tianyuan168326@outlook.com
```
