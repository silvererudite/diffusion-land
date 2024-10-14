# Denoising as Decomposition

I was fascinated by this paper by ["Denoising: A Powerful Building-Block for Imaging, Inverse Problems, and Machine Learning."](https://arxiv.org/abs/2409.06219) by Milanfar et al. 
The main concepts explored here are these:
An image essentially composed of two parts
`X = u + e`


`u` -> the clean image and `e` -> some amount of noise
So X - e which is the residual is essentially the finer details like textures, grainyness, edges added over the smooth image.
In the [Denoising concepts notebook](https://github.com/silvererudite/diffusion-land/blob/main/Denoising/denoising_concepts.ipynb) I explore this concept by gradually denoising an image by applying Gaussian blur and calculating the residuals. 
If we visualize the residuals, we can see that they indeed reveal progressive finer details like textures and edges of the image.
The cool part is that we can use this knowledge to blend different denoisers and also iteratively use different denoisers to create interesting filters or combination of images.


I got so fascinated by this concept that I also built a spin-off [Stable Diffusion residuals](https://github.com/silvererudite/diffusion-land/blob/main/Denoising/ddpm-residual-visualization.ipynb) exploring the residuals to
reveal how the concepts emerge in a diffusion model for text-to-image generation over the steps.
