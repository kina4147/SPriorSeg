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

## Acknowledgement
This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00306, Development of Multimodal Sensor-based Intelligent Sys- tems for Outdoor Surveillance Robots]
