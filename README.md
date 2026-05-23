# 🧵 Fabric Defect Detection

An automated fabric defect detection system comparing three deep learning architectures on the **TILDA (Tianchi Alibaba) textile defect dataset**.

---

## 📌 Problem Statement

Manual quality inspection in textile manufacturing is slow and inconsistent. This project trains and benchmarks object detection / classification models to automatically identify defects in fabric images.

---

## 🏗️ Models Compared

| Model | Task | Approach |
|---|---|---|
| **Swin Transformer** | Classification | Hierarchical vision transformer with shifted windows |
| **Faster R-CNN** | Object Detection | Two-stage region proposal network |
| **EfficientNet** | Classification | Compound scaling of depth, width & resolution |

---

## 📂 Dataset

- **TILDA Textile Dataset** — sourced from Alibaba Tianchi competition
- Contains fabric images labeled with defect regions across multiple defect categories
- Preprocessing: resizing, normalization, augmentation (flips, rotations)

---

## 📁 Repository Structure

```
Fabric_Defect_Detection/
├── swin_transformer.ipynb   # Swin Transformer training & evaluation
├── faster rcnn.ipynb        # Faster R-CNN training & evaluation
├── efficientnet.ipynb       # EfficientNet training & evaluation
└── README.md
```

---

## ⚙️ Setup

```bash
pip install torch torchvision timm albumentations
```

---

## 🔬 Methodology

1. **Data Loading** — Load TILDA images and defect annotations
2. **Preprocessing** — Resize, normalize, and augment images
3. **Model Training** — Train each architecture independently
4. **Evaluation** — Compare mAP / accuracy across models
5. **Analysis** — Identify best-performing architecture per defect category

---

## 📊 Results

| Model | Metric | Score |
|---|---|---|
| Swin Transformer | Accuracy | — |
| Faster R-CNN | mAP | — |
| EfficientNet | Accuracy | — |

> Results to be updated after full training runs.

---

## 🔗 References

- [TILDA Textile Dataset — Tianchi/Alibaba](https://tianchi.aliyun.com/)
- [Swin Transformer Paper (Liu et al., 2021)](https://arxiv.org/abs/2103.14030)
- [Faster R-CNN Paper (Ren et al., 2015)](https://arxiv.org/abs/1506.01497)
- [EfficientNet Paper (Tan & Le, 2019)](https://arxiv.org/abs/1905.11946)

---

## 👤 Author

**Yohan Gala** — B.Tech Computer Engineering, KJSIT Mumbai  
[GitHub](https://github.com/Yohangala)
