## Phase 2 – Foreground Extraction

### Foreground Motion Overlay
![Phase 2 Foreground Motion Overlay](phase2_Foreground%20Motion%20Overlay.png)

This figure visualizes the foreground motion extraction result in Phase 2 of the HiEUM framework. Detected moving regions are overlaid on the original satellite image after background modeling, highlighting candidate areas for further sparse representation and refinement.

---

### Binary Foreground Mask (Ground Truth)
![Phase 2 Binary Ground Truth Mask](phase2_groundtruth_binary_mask.png)

This figure shows the binary foreground mask generated from bounding box annotations. White pixels represent moving objects, while black pixels indicate static background regions. This mask is used for qualitative comparison and intermediate evaluation.

## Phase 3 – Foreground Extraction Refinement

### Refined Foreground Extraction
![Phase 3 Refined Foreground](phase3_foreground_extraction.png)

This figure illustrates the refined foreground extraction results after motion-based filtering. Compared to the previous phase, noise and static background artifacts are reduced, leading to a cleaner representation of moving objects.

## Phase 4 – Sparse Motion Map Generation

### Sparse Motion Map
![Phase 4 Sparse Motion Map](phase4_sparse_map.png)

This figure presents the sparse motion map generated from the extracted foreground regions. The sparsity constraint helps suppress background noise and emphasizes coherent motion patterns corresponding to moving objects.

## Phase 9 – Final Moving Object Detection

### Final Detection Result
![Phase 9 Final Detection](phase9_final_detection.png)

This figure shows the final moving object detection result produced by the HiEUM framework. Detected moving objects are highlighted on the satellite image after iterative refinement and feedback across multiple processing phases.

