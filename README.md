
# Nighttime Pothole Detection

A system that detects potholes in nighttime road images using image processing and deep learning.

## Results

| Model | Accuracy |
|-------|----------|
| Without preprocessing | 61.8% |
| With preprocessing | **83.1%** |

## How It Works

1. **Preprocessing Pipeline:** Convert to grayscale → Log transformation (brightens dark areas) → Laplacian filter (sharpens edges) → Median blur (reduces noise) → Contrast stretching → Overlay with original image
2. **Detection:** TRI-NIT model (via Roboflow)

## Dataset

Nighttime Pothole Dataset (NPD) - 8,740 nighttime road images


## Requirements

```bash
pip install opencv-python numpy matplotlib scikit-image
