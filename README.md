# Image Matching Challenge 2025 

## Overview

This repository contains a modular pipeline for solving the IMC 2025 (Image Matching Challenge) using a hybrid of DINO, SuperPoint, LightGlue, and COLMAP. The core goal was to cluster images by 3D scene, match keypoints robustly, and reconstruct poses via Structure-from-Motion.

## Features
- Global Scene Clustering using DINOv2 ViT and FAISS + Louvain
- Local Keypoint Matching using SuperPoint & LightGlue
- RANSAC-based match validation
- COLMAP-compatible SfM reconstruction
- Adaptive thresholding using scene-specific thresholds from train_thresholds.csv
- Compatible with IMC scoring and evaluation (metric.py)

## Dataset Used
- https://www.kaggle.com/competitions/image-matching-challenge-2025/data
- https://www.kaggle.com/datasets/eduardtrulls/imc25-utils

## Acknowledgements
- https://colmap.github.io/index.html
- https://github.com/cvg/LightGlue
- Leroy, Vincent, Yohann Cabon, and Jérôme Revaud. "Grounding image matching in 3d with mast3r." In European Conference on Computer Vision, pp. 71-91. Cham: Springer Nature Switzerland, 2024.
- Murez, Zak, Tarrence Van As, James Bartolozzi, Ayan Sinha, Vijay Badrinarayanan, and Andrew Rabinovich. "Atlas: End-to-end 3d scene reconstruction from posed images." In European conference on computer vision, pp. 414-431. Cham: Springer International Publishing, 2020.
