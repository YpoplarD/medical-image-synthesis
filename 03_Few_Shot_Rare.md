# Few-Shot & Rare Disease Synthesis

Methods designed for **extreme data imbalance**, **anatomy manipulation**, and **generating hard-to-acquire pathologies**.

* `AnoDDPM` [Wyatt et al., Proc. TMI 2022] **AnoDDPM: Anomaly Detection with Denoising Diffusion Probabilistic Models using Simplex Noise** [[PDF]](https://ieeexplore.ieee.org/document/9857019) [[CODE]](https://github.com/Julian-Wyatt/AnoDDPM)
  
  只学习健康数据，使用单纯形噪声
* `DeltaGAN` [Yan Hong et al., Proc. CVPR 2022] **DeltaGAN: Towards Diverse Few-shot Image Generation with Sample-Specific Delta** [[PDF]](https://arxiv.org/pdf/2009.08753) [[CODE]](https://github.com/bcmi/DeltaGAN-Few-Shot-Image-Generation)

  通用领域，从健康数据中学习变换（即不同健康个体之间的差别），再作用到小样本上以扩充数据量。（例：模型学习一个瘦的人、胖的人、正常身材的人的某个部位，之后将一张带病灶的样本扩充为这三种情况的三张/）
* `DAA-GAN` [Thermos et al., IEEE TMI 2021] **Controllable cardiac synthesis via disentangled anatomy arithmetic** [[PDF]](https://arxiv.org/abs/2107.01748v1) [[CODE]](https://github.com/vios-s/DAA-GAN)

  解剖和重构，将病变区域“移植”到健康数据上
* `DiffAug` [Jiaying Zhang et al., TMI 2024] **Data Augmentation in Class-Conditional Diffusion Model for Semi-Supervised Medical Image Segmentation** [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10650822)
  
  在健康图上放病灶，利用筛选机制留下合理的
