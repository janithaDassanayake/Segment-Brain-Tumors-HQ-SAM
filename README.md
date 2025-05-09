# 🧠 HQ-SAM Brain Tumor Segmentation

This project demonstrates the use of **HQ-SAM (High-Quality Segment Anything Model)** to perform **fine-grained brain tumor segmentation** on MRI images. It leverages the enhanced capabilities of Meta's SAM-HQ model via the Hugging Face `transformers` library to produce accurate segmentation masks from simple prompts like 2D points or bounding boxes.


---

## 📸 Example: Tumor Mask Prediction from a 2D Point

![Tumor Segmentation Demo](https://github.com/janithaDassanayake/dummyimages/raw/main/ezgif-6d2ae22bc42f05%20\(1\)%20\(1\).gif)

A single point inside the tumor region is enough to generate a high-quality segmentation mask. The model can also return multiple masks with associated IoU scores for flexibility in medical review.

---

## 📌 Key Features

* 🔬 Medical application: Brain tumor localization from MRI scans
* ⚡ Efficient inference using pre-computed embeddings
* 🎯 Multiple prompting strategies:

  * Single or multiple 2D points
  * Bounding boxes
  * Combined points + boxes
* 🖼️ Support for visualizing masks, boxes, and prompts

---


## 🚀 Try It on Google Colab

👉 **Run the notebook instantly via Colab**:
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1iEhxEvGMN9TxdFafszb_Vnybo9h_AVnl?usp=sharing)

---

## 🔍 Use Cases Explained

### ✅ Use Case 1: Point-Based Prompting

Generate masks from one or more 2D points inside the tumor region.

![Tumor Center](https://github.com/janithaDassanayake/dummyimages/blob/main/b1.png?raw=true)

### ✅ Use Case 2: Bounding Box Prompting

Guide the segmentation using a bounding box—ideal for coarse targeting.

![Bounding Box](https://github.com/janithaDassanayake/dummyimages/blob/main/b2.png?raw=true)
### ✅ Use Case 3: Combined Prompts

Combine both a point and a bounding box for more precise results.

![Segmentation Masks](https://github.com/janithaDassanayake/dummyimages/blob/main/b3.png?raw=true)
### ✅ Use Case 4: Multi-Region Segmentation

Feed multiple prompts to generate multiple masks per image (e.g., multi-focal tumors).

![Final Output](https://github.com/janithaDassanayake/dummyimages/blob/main/b4.png?raw=true)
---


### 🔄 Adaptable Use Cases

Here are a few examples where this pipeline can be applied with minimal modification:

### 🧬 Medical Imaging

* **Lung nodule segmentation** in chest CT scans
* **Retinal lesion detection** in fundus images
* **Skin lesion segmentation** in dermoscopic images
* **Polyp segmentation** in colonoscopy frames

### 🧠 General Image Segmentation

* **Object extraction** in satellite images (e.g., roads, buildings, vegetation)
* **Instance segmentation** in industrial quality control (e.g., detecting defects in machinery or PCBs)
* **Animal and organ segmentation** in veterinary or biological datasets

> With only a few prompt modifications (points or bounding boxes), HQ-SAM can generalize remarkably well across domains.

## 📚 References

* [SAM Paper (Meta, 2023)](https://ai.facebook.com/research/publications/segment-anything/)
* [HQ-SAM GitHub](https://github.com/SysCV/sam-hq)
* [Hugging Face Model Hub](https://huggingface.co/syscv-community)
* [Original Hugging Face Notebook](https://github.com/huggingface/notebooks/blob/main/examples/segment_anything.ipynb)

---

## 🤝 Acknowledgements

Special thanks to:

* **Meta AI** for developing SAM and HQ-SAM
* **Hugging Face** for enabling model access via `transformers`
* Community contributors to SAM-HQ notebook
