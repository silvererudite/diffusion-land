# Implementaion of Denoising diffusion probabilistic model in pytorch

Dataset:
- Oxford flowers
- num epochs: 50
I replaced the original U-Net mentioned in the paper with a custom CNN (just for fun)

Observations:
- num of epochs needed to denoise is propostional to `noise_std` value
- the denoised version tends towards blurry photos even after 50 epochs
  
