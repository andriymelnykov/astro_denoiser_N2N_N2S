# Astro Denoiser Noise2Noise and Noise2Stack hybrid

This is a script to train neuronal network based noise filter for astro images.
It implements an idea of Noise2Noise training, described here:
"Noise2Noise: Learning Image Restoration without Clean Data", Jaakko Lehtinen, Jacob Munkberg, Jon Hasselgren, Samuli Laine, Tero Karras, Miika Aittala, Timo Aila;
and Noise2Stack, derived from:
"Learning to denoise astronomical images with U-nets", Vojtekova, Antonia; Lieu, Maggie; Valtchanov, Ivan; Altieri, Bruno; Old, Lyndsay; Chen, Qifeng; Hroch, Filip


The script Astro_Denoiser_N2N_N2S.ipynb can be used for Noise2Noise, Noise2Stack or hybrid training.
If you want to use Noise2Noise only, use dummy images as stacks in the dataset structure.

The script Image_Denoiser.ipynb can be used to test a trained model on a big image (TIFF, RGB, 16bit).

Both scripts are designed to run in Google Colab.

The pre-trained models are in the folder "trained_models". These models are used in my Digital_Eyepiece_APP software, see my other repositories. These are trained on my own images, with a goal to be effective with my optics/camera/image processing, and are not neccessary effective on other images.

The whole dataset used for training is available here: https://drive.google.com/drive/folders/16YdNMLbarSQggHxbmVOwAh6BR7b2nApB?usp=sharing
The images in the dataset are/(should be) TIFF, RGB, 16bit, calibrated, with background compensation, with same nonlinear stretching for each object.

95% of the code is written by ChatGPT o3.

Andriy Melnykov, 2025
