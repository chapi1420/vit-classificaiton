# 🧠 Vision Transformer (ViT) for CIFAR-10 Image Classification

This project demonstrates an **advanced implementation of the Vision Transformer (ViT)** using PyTorch, applied to the CIFAR-10 dataset. It includes:

- Hands-on implementation from patch embedding to MLP head
- Transformer encoder block logic with multi-head self-attention
- Hyperparameter tuning and model training across multiple epoch settings
- Detailed training logs, performance plots, and model checkpointing

---

## 📁 Project Structure

```
vit-cifar10/
├── notebook/                 # Main Jupyter Notebook implementation
├── .vscode/                  #basic setting configurations
├──.github/
├──src/                       #empty as project done or google colab
├──scripts/                   #empty as project done using google colab
├── vit_training.log          # Log of all training runs
├── vit_checkpoints.zip       # Zipped model checkpoints (10, 20, 30 epochs)
├── plots/                    # (Optional) Training plots for loss & accuracy
└── README.md                 # Project overview (this file)
```

---

## 🚀 Key Features

- ✅ **Patch Embedding** with `[CLS]` token and positional encodings
- ✅ **Transformer Encoder Block** with multi-head attention, MLP, and layer norm
- ✅ **MLP Head** for 10-way classification
- ✅ **Training Loops** with `AdamW`, cosine learning rate scheduling, and checkpoint saving
- ✅ **Validation Accuracy Tracking** and plots
- ✅ **Log File** recording all experiments and metrics

---

## 📊 Experiment Settings

We trained ViT on CIFAR-10 using the following epoch settings:

| Epochs | Best Val Accuracy |
| ------ | ----------------- |
| 10     | 0.7098            |
| 20     | 0.7754            |
| 30     | 0.8093            |

> Replace `XX.XX%` with your actual best validation accuracy per run.

All models were saved as `.pth` files, and logs were stored for reproducibility.

---

## 📦 Requirements

- Python 3.8+
- PyTorch
- torchvision
- matplotlib
- tqdm

### ✅ Install locally

```bash
pip install torch torchvision matplotlib tqdm
```

If running on Google Colab, all dependencies are already installed.

---

## 📥 Usage

### 🧪 Inference on Validation Images

Run this inside your notebook to visualize predictions:

```python
show_predictions(model, val_loader, device)
```

### 🔁 Train With Different Epochs

Change this list to explore various training durations:

```python
epoch_options = [10, 20, 30]
```

### 🧠 Conceptual Understanding

This project is accompanied by a theoretical presentation covering:

- Vision Transformer (ViT) architecture
- Image patching & embedding
- Self-attention and multi-head attention
- Positional encoding
- Residual connections & layer normalization
- Why ViT is data-hungry and the value of pretraining

---

## 📜 License

This project is for educational and non-commercial use.

---

## 🙋‍♂️ Author

Nahom Temesgen Nadew (Mohan)  
Intern at iCog Labs  
Machine Learning and Computer Vision Enthusiast
