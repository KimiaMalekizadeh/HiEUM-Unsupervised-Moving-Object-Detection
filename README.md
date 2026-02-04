# HiEUM: Unsupervised Moving Object Detection (Re-implementation)

This repository contains an educational and qualitative re-implementation of the paper:

**Highly Efficient and Unsupervised Framework for Moving Object Detection in Satellite Videos**  
Chao Xiao et al., IEEE TPAMI.

## Overview
This project reproduces the main algorithmic pipeline of the HiEUM framework, including:
- Dataset reduction for hardware-limited environments
- Background modeling and motion extraction
- Initial sparse representation
- Pseudo-label generation and refinement
- Iterative self-evolution and sparse feedback
- Final moving object detection

The implementation focuses on qualitative analysis and algorithmic understanding rather than quantitative benchmarking.

## Original Work
- Official paper and code: https://github.com/ChaoXiao12/Moving-object-detection-in-satellite-videos-HiEUM

## Project Structure

The implementation is organized into sequential Jupyter notebooks,
each corresponding to one phase of the HiEUM framework:

- **Phase 0**: Dataset Reduction  
- **Phase 1**: Preprocessing  
- **Phase 2**: Background Modeling  
- **Phase 3**: Motion / Foreground Extraction  
- **Phase 4**: Sparse Motion Representation  
- **Phase 5**: Pseudo-label Generation  
- **Phase 6**: Label Refinement  
- **Phase 7**: Self-Evolution  
- **Phase 8**: Sparse Feedback  
- **Phase 9**: Final Detection  

All notebooks are located in the `notebooks/` directory and should be executed in order.

## Disclaimer
This is **not the official implementation**.  
All credits for the original method belong to the authors.

## Qualitative Results

Below are qualitative results from different phases of the HiEUM pipeline:

### Foreground Extraction and Motion Overlay (Phase 2)
This figure illustrates the foreground extraction result of Phase 2, where moving regions are highlighted and overlaid on the original satellite frame. The foreground mask is obtained through background modeling and subtraction, allowing candidate motion regions to be separated from the static background. This step serves as a crucial pre-processing stage for subsequent sparse representation and motion refinement phases.


### Binary Ground Truth Mask 
![Ground Truth Mask](fig_groundtruth_binary_mask.png)

This binary mask is generated from dataset bounding box annotations and is used only for qualitative comparison with the unsupervised detection results.

### Phase 3 – Foreground Extraction
![Phase 3](figures/phase3_foreground_extraction.png)

### Phase 4 – Sparse Motion Map
![Phase 4](figures/phase4_sparse_map.png)

### Phase 6 – Refinement
![Phase 6](figures/phase6_refinement.png)

### Phase 9 – Final Moving Object Detection
![Phase 9](figures/phase9_final_detection.png)
