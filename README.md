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
@article{ibrahim2023unloc,
  title={UnLoc: A Universal Localization Method for Autonomous Vehicles using LiDAR, Radar and/or Camera Input},
  author={Ibrahim, Muhammad and Akhtar, Naveed and Anwar, Saeed and Mian, Ajmal},
  journal={arXiv preprint arXiv:2307.00741},
  year={2023}
}

@ARTICLE{10046141,
  author={Ibrahim, Muhammad and Akhtar, Naveed and Anwar, Saeed and Mian, Ajmal},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={SAT3D: Slot Attention Transformer for 3D Point Cloud Semantic Segmentation}, 
  year={2023},
  volume={24},
  number={5},
  pages={5456-5466},
  doi={10.1109/TITS.2023.3243643}}

@article{ibrahim2023slice,
  title={Slice Transformer and Self-supervised Learning for 6DoF Localization in 3D Point Cloud Maps},
  author={Ibrahim, Muhammad and Akhtar, Naveed and Anwar, Saeed and Wise, Michael and Mian, Ajmal},
  journal={arXiv preprint arXiv:2301.08957},
  year={2023}
}
```
