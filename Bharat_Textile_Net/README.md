# Bharat Textile Net
### Traditional Textile Pattern Recognition Dataset

> **Course:** CSE3292 — Deep Learning for Computer Vision  
> **Project Domain:** Traditional Textile Pattern Recognition  
> **Date:** January 2026  

---

# Team Members

| Name | Roll Number |
|-----|-----|
| Hardik Jain | 23ucs583 |
| Akkshit Gupta | 23ucs523 |
| Abhinav Thulal | 23ucs508 |
| Ayush Verma | 23ucs552 |
| Bhagya Dhingra | 23ucs553 |

---

# Overview

**Bharat Textile Net** is a curated computer vision dataset designed for recognizing **traditional Indian textile patterns and clothing styles**.

Many popular datasets used in computer vision research focus on **generic textures or Western fashion categories**. As a result, models trained on them often struggle to identify **fine-grained Indian textile patterns**, which involve unique weaving, dyeing, embroidery, and printing techniques.

This dataset addresses that gap by providing **a culturally relevant benchmark for Indian textile recognition**.

The dataset is intended for:

- Image classification
- Textile pattern recognition
- Cultural fashion AI
- Transfer learning experiments
- Deep learning research on Indian fabrics

---

# Motivation

Most computer vision datasets such as:

- Describable Textures Dataset (DTD)
- DeepFashion
- Fashion-MNIST

do not adequately represent **Indian textile traditions**.

However, Indian fabrics include highly distinctive styles such as:

- block printing
- tie-dye patterns
- silk brocade weaving
- handloom textures
- embroidery-based motifs

Because of this lack of representation, deep learning models often fail to recognize **fine-grained Indian textile patterns**.

Our goal is to create a **benchmark dataset for Indian textile recognition** that improves model understanding of these culturally significant patterns.

---

# Dataset Summary

| Attribute | Value |
|---|---|
| Total Images | ~2000–2500 |
| Number of Classes | 10 |
| Images per Class | ~200–250 |
| Image Format | JPEG (.jpg) |
| Dataset Type | Image Classification |
| Annotation Format | CSV |

Each team member collected approximately **400–500 images**, making the dataset feasible to construct within the project timeline.

---

# Dataset Classes

The dataset includes **10 traditional textile and garment pattern categories**.

Examples of textile styles represented include:

- Kalamkari
- Ikat
- Pashmina
- Ajrakh
- Chikankari

These styles represent **different Indian regions, weaving techniques, and cultural traditions**.

---

# Dataset Sources

Images were collected from multiple publicly accessible sources.

### Image Search Platforms
- Google Images (Creative Commons filter)
- Flickr (CC-licensed images)

### E-Commerce Catalogs
- Myntra
- IndiaMart
- FabricPedia
- VrikshamIndia
- KalamkariBlockPrints
- Soovos Handlooms
- JSP Handlooms

### Cultural & Archive Sources
- Museum textile collections
- Craft archives
- Handloom documentation portals

These sources ensure a mixture of:

- catalog images
- real-world fabric photographs
- museum documentation images

This diversity improves dataset robustness.

---

# Image Naming Convention

Each image follows the format:

```
class_source_index.jpg
```

Example:

```
ikat_flickr_012.jpg
kalamkari_google_041.jpg
bandhani_indiamart_023.jpg
```

This naming structure preserves information about:

- class label
- data source
- unique identifier

---

# Annotation Format

Metadata for each image is stored in a CSV file.

```
image_id,filename,label,source,license
1,ikat_flickr_012.jpg,Ikat,Flickr,CC-BY
2,kalamkari_google_041.jpg,Kalamkari,Google Images,CC
```

Fields include:

| Field | Description |
|---|---|
| image_id | Unique image identifier |
| filename | Image file name |
| label | Textile pattern category |
| source | Website or archive where image was obtained |
| license | Usage license (where available) |

---

# Annotation Strategy

To ensure annotation quality, a structured annotation protocol was followed.

### Step 1 — Reference Guidelines
Each class was defined using **reference images and short visual descriptions**.

### Step 2 — Multi-Annotator Validation
The first **100 images were labeled by multiple annotators** to check consistency and agreement.

### Step 3 — Rule Refinement
Disagreements were discussed and class definitions refined.

### Step 4 — Distributed Annotation
Remaining images were divided among team members for labeling.

---

# Data Cleaning

During dataset preparation, the following images were removed:

- blurry images
- heavily edited images
- low resolution photos
- images where **fabric coverage was less than 40%**

This ensures the dataset focuses on **clear textile patterns**.

---

# Ethical Considerations

### Privacy
Images were sourced from **publicly available datasets and catalogs**.

No private photographs were included.

### Licensing
Where possible, images were selected using:

- Creative Commons filters
- public archives
- research-use catalog images

### Face Privacy
If faces appeared in images, they were **cropped or blurred**.

---

# Dataset Diversity

The dataset includes images from:

- multiple Indian regions
- different weaving traditions
- catalog photographs
- real-world fabric images

Variation includes:

- lighting conditions
- background complexity
- fabric folds
- scale differences

This diversity helps improve model generalization.

---

# Project Timeline

The dataset was constructed over **6 weeks**.

| Week | Task |
|---|---|
| Week 1–2 | Image collection |
| Week 3–4 | Data cleaning and annotation |
| Week 5 | Dataset splitting |
| Week 6 | Documentation and evaluation |

With **5 team members collecting 400–500 images each**, the target dataset size was achievable.

---

# Applications

This dataset can support research in:

- textile pattern classification
- cultural garment recognition
- fashion recommendation systems
- heritage textile documentation
- deep learning based fashion search

---

# Limitations

- Some classes may share visual similarities
- Background clutter may appear in real-world images
- Dataset size is moderate compared to large benchmarks

Future work may include:

- segmentation masks
- object detection annotations
- larger dataset expansion

---

# Citation

```
Bharat Textile Net: Traditional Textile Pattern Recognition Dataset
CSE3292 — Deep Learning for Computer Vision
January 2026
```

---
