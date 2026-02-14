# Beyond Raw Accuracy: Emotion Recognition with Random Projection

This project presents a progressive deep learning framework for facial emotion recognition, integrating cross-attention mechanisms and Random Projection for efficient feature representation.

## 📌 Overview

The system performs multi-class facial emotion classification across five emotion categories:

- Angry  
- Fear  
- Happy  
- Sad  
- Surprise  

The architecture evolves through three stages:

1. Baseline CNN (ReLU + Adam)
2. Improved model with Glue activation and Cross-Attention
3. Final proposed model integrating Random Projection for dimensionality reduction

The final architecture achieved **94% classification accuracy**.

## 🧠 Key Contributions

- EfficientNet-B0 backbone for deep feature extraction
- Cross-attention mechanism to capture emotionally salient regions
- Glue activation function for improved gradient propagation
- Random Projection for lightweight dimensionality reduction
- Reduced computational complexity while preserving geometric structure

## 📊 Model Evolution

| Model | Components | Accuracy |
|-------|------------|----------|
| Baseline | ReLU + Adam | 84% |
| Improved | Glue + Cross-Attention + ClipNorm | 92% |
| Proposed | Random Projection + Cross-Attention | 94% |

## 🛠 Tools & Technologies

- Python
- TensorFlow / Keras
- EfficientNet-B0
- NumPy
- Matplotlib

## ⚙️ Training Configuration

- Image size: 300x300
- Optimizer: Adam
- Learning rate: 5e-5
- Gradient clipping (ClipNorm = 1.0)
- Two-phase training (freeze + fine-tuning)

## 📂 Dataset

Custom-collected and manually annotated facial emotion dataset.

---

This project was developed as part of a Pattern Recognition course at the University of Jordan.
