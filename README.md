# 3D Gaussian Splatting - Chair Reconstruction

This project reconstructs a real-world chair as an interactive 3D scene using Gaussian Splatting. The entire pipeline runs from a phone video to a fully navigable 3D model.

## Pipeline

1. Filmed the chair with a phone from multiple angles
2. Extracted frames using ffmpeg (1 frame per second)
3. Ran COLMAP for camera pose estimation and sparse reconstruction
4. Trained a Gaussian Splatting model on Google Colab (T4 GPU)
5. Visualized the result in SuperSplat

## Result

![demo](https://github.com/FJvEngelen/gaussian-splatting-chair/raw/main/point_cloud.mp4)

428,759 splats reconstructed from 61 frames.

## Why this matters

Gaussian Splatting is the same technology used in VFX pipelines for scene reconstruction and virtual production. This experiment was a first step in understanding how real-world capture translates into 3D representations that can be used in film, games, and AR/VR.

## Tools used

- ffmpeg
- COLMAP
- gaussian-splatting (graphdeco-inria)
- Google Colab
- SuperSplat (PlayCanvas)
