# Flower Metric Learning Project

A metric learning project for flower classification using DINOv2, achieving **99%+ ROC-AUC** on Oxford 102 Flowers dataset.

## 🏆 Results
- **ROC-AUC: 99%+** on flower similarity search
- **Precision@1: 99%+** for finding similar flowers
- **Training time: ~8 minutes** per model

## 🚀 Quick Start

```python
# Install requirements
pip install torch torchvision timm pytorch-lightning pytorch-metric-learning
pip install albumentations opencv-python matplotlib scikit-learn tqdm

# Run the notebook/script
# All steps are included: dataset download, training, evaluation, demo
```

## ✨ Features
- Automatic Oxford 102 Flowers dataset download
- DINOv2-based embedding network
- Two loss strategies: Center Loss vs Combined Loss
- Interactive similarity search demo
- Comprehensive evaluation with ROC-AUC
- Cross-domain testing on real fruit images

## 📊 What's Included
1. **Environment setup** with GPU optimization
2. **Dataset preparation** (8,189 flower images, 102 classes)
3. **Model training** with two different loss functions
4. **Evaluation** with ROC-AUC and precision metrics
5. **Interactive demo** for similarity search
6. **Robustness testing** against noise and transformations
7. **Cross-domain testing** on real fruit images

## 🎮 Interactive Demo
The project includes an interactive demo where you can:
- Select any flower image
- Find the most similar flowers
- Compare different models
- See t-SNE visualizations

## 🔬 Technical Details
- **Backbone**: DINOv2-Small pre-trained model
- **Architecture**: 384D → 512D embedding with L2 normalization
- **Loss Functions**: Center Loss (intra-class) + Proxy Anchor/NCA (inter-class)
- **Training**: AdamW optimizer with cosine annealing
- **Evaluation**: ROC-AUC, Precision@K, embedding quality analysis

## 📈 Architecture
```
Input (224x224 RGB) → DINOv2 Backbone → Projection Head → L2 Normalize → 512D Embedding
```

## 🎯 Use Cases
- Flower species identification
- Botanical research and classification
- Image similarity search systems
- Educational tools for flower recognition

## 📝 How to Run
Just run all cells in the notebook/script - everything is automated:
- Dataset downloads automatically
- Models train and save checkpoints
- Evaluation runs and shows results
- Interactive demo launches at the end

Perfect for Google Colab! 🚀
