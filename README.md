# Quad-Tree-Based Driver Classification for MCI Detection

This repository contains the official implementation of the paper:

**Quad-Tree-Based Driver Classification Using Deep Learning for Mild Cognitive Impairment Detection**  
*IEEE Access, 2025*  
DOI: 10.1109/ACCESS.2025.3558706

## Overview
We propose a geo-regional quad-tree framework for transforming raw GPS trajectories into hierarchical spatial representations. These representations are encoded into binary features and used as input to a 2D Convolutional Neural Network (CNN) to classify drivers as cognitively normal or mildly cognitively impaired (MCI).

The proposed approach:
- Preserves spatial hierarchy of trajectories
- Avoids aggressive feature aggregation
- Achieves up to **95% F1-score** on real-world telematics data

## Repository Structure
- `src/quadtree/` – Quad-tree construction and binary encoding
- `src/models/` – CNN architecture and training pipeline
- `src/preprocessing/` – GPS processing and segmentation
- `data/synthetic/` – Example data (no real participant data)
- `experiments/` – Reproducible experiment scripts

## Data Availability
Due to privacy and IRB restrictions, real GPS and telematics data used in the study cannot be shared.  
This repository includes **synthetic examples** to demonstrate the full pipeline.

## Requirements
```bash
pip install -r requirements.txt
