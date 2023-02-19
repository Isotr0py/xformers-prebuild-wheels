# xformers-prebuild-wheels
xformers prebuild wheels for Tesla T4 and P100 GPU, developed in and for kaggle notebook environment.

All wheels were tested on [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) in kaggle notebook environment.

## Prebuild
Just select your python verison in `xformers_any_cp.ipynb`:
```
!conda create -y -n LoRA python=3.10 
!conda run -n LoRA python --version
```
Then run it in kaggle. It may cost about 2 hours for wheel building. 

As the cuda version in kaggle is 11.2, all wheels are built with `torch==1.12.1+cu113` and `torchvision==0.13.1+cu113`.