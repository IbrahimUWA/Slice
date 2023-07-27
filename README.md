# Slice Transformer and Self-supervised Learning for 6DoF Localization in 3D Point Cloud Maps

This repository is for transformer based self-supervised localization method and dataset introduced in the following paper

[Muhammad Ibrahim,  Naveed Akhtar,  Saeed Anwar, Michael Wise and  Ajmal Mian, "[Slice Transformer and Self-supervised Learning for 6DoF Localization
in 3D Point Cloud Maps]", IEEE International Conference on Robotics and Automation (ICRA), 2023

## Contents
1. [Introduction](#introduction)
2. [Requirements](#requirements)
3. [Citation](#citation)
4. [Acknowledgements](#acknowledgements)

## Introduction
Precise localization is critical for autonomous vehicles. We present a self-supervised learning method that employs transformers for the first time for the task of outdoor localization using LiDAR data. We propose a pre-text task that reorganizes the slices of a $360^\circ$ LiDAR scan to leverage its axial properties. Our model, called Slice Transformer, employs multi-head attention while systematically processing the slices. To the best of our knowledge, this is the first instance of leveraging multi-head attention for outdoor point clouds. We additionally introduce the Perth-WA dataset, which provides a large-scale LiDAR map of Perth city in Western Australia, covering $\sim$4km$^2$ area. Localization annotations are provided for Perth-WA.  The proposed localization method is thoroughly evaluated on Perth-WA and Appollo-SouthBay datasets. We also establish the efficacy of our self-supervised learning approach for the common downstream task of object classification using ModelNet40 and ScanNN datasets. The code and Perth-WA data will be publicly released.


## Requirements
- PyTorch 0.4.0, PyTorch 0.4.1 
- Tested on Ubuntu 14.04/16.04 environment 
- torchvision=0.2.1
- python 3.6
- CUDA 9.0 
- cuDNN 5.1 
- imageio
- pillow
- matplotlib
- tqdm 
- scikit-image

---

---

## Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@article{Anwar2021R2NET,
    title={Attention Prior for Real Image Restoration},
    author={Saeed Anwar and Nick Barnes and Lars Petersson},
    journal={IEEE Transactions on Neural Networks and Learning Systems (TNNLS)},
    year={2021}

}

@article{anwar2019ridnet,
  title={Real Image Denoising with Feature Attention},
  author={Anwar, Saeed and Barnes, Nick},
  journal={IEEE International Conference on Computer Vision (ICCV-Oral)},
  year={2019}
}

@article{Anwar2020IERD,
  author = {Anwar, Saeed and Huynh, Cong P. and Porikli, Fatih },
    title = {Identity Enhanced Image Denoising},
    journal={IEEE Computer Vision and Pattern Recognition Workshops (CVPRW)},
    year={2020}
}
```
