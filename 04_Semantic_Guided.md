# Text / Semantic-Guided Synthesis

Methods leveraging priors (segmentation masks, text prompts, biological attributes) for **controllable generation** or **generative segmentation**.
* `MedSegDiff` [Wu et al., Proc. ICLR 2023] **MedSegDiff: Medical image segmentation with diffusion models** [[PDF]](https://arxiv.org/abs/2301.11798v2) [[CODE]](https://github.com/ImprintLab/MedSegDiff?tab=readme-ov-file)
  
从原图生成分割掩码，对皮肤镜需要后处理，否则会出现伪影，对CT/MRI等黑底图片采样五次情况下分割效果良好，但耗时过久（3分钟左右生成一张），仅采样一次情况下效率虽然提示但效果有明显下滑，但仍然表现尚可。
* `SegGuidedDiff` [Konz et al., Proc. MICCAI 2024] **Anatomically-controllable medical image generation with segmentation-guided diffusion models** [[PDF]](https://arxiv.org/abs/2402.05210) [[CODE]](https://github.com/mazurowski-lab/segmentation-guided-diffusion)
  
从病灶掩码反向生成原始图像，在皮肤镜数据集上表现较差，容易出现奇怪颜色的背景，在CT/MRI上无此类问题，ROI一致性高，但生成细节容易出现问题（如生成弯曲的刻度线）。
