# CNN-Ship-Classifier
A full end-to-end image classification pipeline written entirely in Perl.

---
---
## **Overview**

This repository contains a complete implementation of a Convolutional Neural Network (CNN) in **Perl**, built to classify satellite/aerial images of **ships vs. non-ships**.

The entire workflow —dataset loading, preprocessing, tensor conversion, CNN architecture, training loop, learning-rate scheduling, early stopping, metrics, and visualizations— is implemented using modules from the Perl ecosystem:

- **AI::MXNet** (deep learning)
- **PDL** (tensors / numerical computing)
- **Imager** (image loading)
- **Chart::Plotly** (visualization)
- **IPerl** (Jupyter kernel for Perl)

Plus a set of **reusable custom modules**:

- `ImageFolderDataset.pm`
- `ImageFolderDatasetSubset.pm`
- `DataLoader.pm`
- `ConfusionMatrixPlot.pm`

This project serves as a practical demonstration of *modern machine learning in Perl* — no Python required.

---

## **Features**

✔ Mini-VGG style CNN architecture  
✔ SoftmaxCrossEntropy loss  
✔ Adam optimizer  
✔ Learning Rate Scheduler  
✔ Early Stopping  
✔ Batch-level F1-score  
✔ Macro F1 per epoch  
✔ Confusion Matrix visualization  
✔ Plotly training curves  
✔ Full interactive IPerl notebook  

---

## **Installation**

### Requirements
- Perl 5.30+
- PDL
- AI::MXNet >= 1.6 (from source)
- Imager
- Chart::Plotly
- IPerl (optional, for the notebook)

### Install IPerl
```bash
cpanm IPerl
iperl notebook
