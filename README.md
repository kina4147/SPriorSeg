# SemanticPriorSeg

<b>Fast Road-Object Segmentation using Deep Semantic Prior for Sparse 3D Point Cloud (SMC 2020)</b>

This repository contains the official python implementation for our full paper at IROS 2020 "[3D Multi-Object Tracking: A Baseline and New Evaluation Metrics](http://www.xinshuoweng.com/papers/AB3DMOT/camera_ready.pdf)" and short paper "[AB3DMOT: A Baseline for 3D Multi-Object Tracking and New Evaluation Metrics](http://www.xinshuoweng.com/papers/AB3DMOT_eccvw/camera_ready.pdf)" at ECCVW 2020. Our project website and video demos are [here](http://www.xinshuoweng.com/projects/AB3DMOT/). If you find our paper or code useful, please cite our papers:

```
@article{Na2020SMC_SemanticPriorSeg, 
author = {Ki-In Na, Byungjae Park and Jong-Hwan Kim}, 
journal = {SMC}, 
title = {{Fast Road-Object Segmentation using Deep Semantic Prior for Sparse 3D Point Cloud}}, 
year = {2020} 
}
```

<img align="center" src="https://github.com/xinshuoweng/AB3DMOT/blob/master/main.gif">

## Overview
- [News](#news)
- [Introduction](#introduction)
- [Dependencies](#dependencies)
- [3D Object Detection](#3d-object-detection)
- [3D Multi-Object Tracking](#3d-multi-object-tracking)
- [Acknowledgement](#acknowledgement)

## Introduction
Detection and classification of road-objects like cars, pedestrians, and cyclists is the first step in autonomous driving. Especially, point-wise object segmentation for a 3D point cloud is essential to estimate road-objects’ precise ap- pearance. This paper proposes fast and accurate point-level object segmentation using deep semantic cue for point cloud by integrating the strengths of deep convolutional auto-encoder and region growing algorithm. CNN-based semantic segmenta- tion labels a spherical projection image of point cloud pixel- by-pixel to types of road-objects. The connected component method achieves pixel-wise instance segmentation by taking into account geometric and semantic features between neighboring pixels. We extract point-wise labeled datasets for types and objects from 3D bounding boxes and point clouds in the KITTI object dataset. The dataset is employed to train a neural network for semantic segmentation and demonstrate both semantic and instance segmentation’s performance.

## Datasets
We built our dataset including pixel-wise semantic and instance labeled channels from the KITTI object dataset through the same process as
described in SqueezeSeg. Our dataset is well-balanced for all the classes: a pedestrian, car, and cyclist. 3D bounding boxes of the KITTI object dataset are annotated on the front camera image, and the 3D point cloud is from Velodyne HDL-64E LiDAR with 64 channels. Therefore, the dataset has 512 grids between −45deg and 45deg in the row direction and 64 grids between −24.8deg and 2deg in the column direction. You can download dataset [here](https://drive.google.com/u/1/uc?export=download&confirm=a9LV&id=1bKoXBmF0epHpmQ3E-G_IFABrRid_l3P8)

## Acknowledgement
This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00306, Development of Multimodal Sensor-based Intelligent Sys- tems for Outdoor Surveillance Robots]

https://drive.google.com/u/1/uc?export=download&confirm=a9LV&id=1bKoXBmF0epHpmQ3E-G_IFABrRid_l3P8
