# xformers-prebuild-wheels
xformers prebuild wheels for Tesla T4 and P100 GPU, developed in and for kaggle notebook environment.

All wheels were tested on [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) in kaggle notebook environment.

## Prebuild
Just run `xformers_prebuild.ipynb` in kaggle.

## Install
Before install xformers, run 

`pip install torch==1.12.0+cu113 torchvision==0.13.0+cu113 --extra-index-url https://download.pytorch.org/whl/cu113`

to update pytorch and torchvision to support xformers.

## Tesla T4, Python 3.7 and Cuda11.3(Default in kaggle)
Thanks to [stable-diffusion-webui-colab](https://github.com/camenduru/stable-diffusion-webui-colab), their wheel for colab T4 works well in kaggle.

`pip install https://github.com/camenduru/stable-diffusion-webui-colab/releases/download/0.0.14/xformers-0.0.14.dev0-cp37-cp37m-linux_x86_64.whl`

## P100, Python 3.7 and Cuda11.3(Default in kaggle)
`pip install https://github.com/Isotr0py/xformers-prebuild-wheels/raw/main/P100/xformers-0.0.14.dev0-cp37-cp37m-linux_x86_64.whl`
