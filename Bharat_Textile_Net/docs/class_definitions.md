# Bharat Textile Net: Class Definitions

This document defines the **visual characteristics, inclusion criteria, and annotation guidelines** for each class in the **Bharat Textile Net dataset**.

The dataset focuses on **traditional Indian textile patterns and fabric techniques**, enabling machine learning models to recognize culturally significant textile styles.

Annotations are based on **visual textile patterns and fabric characteristics**, not the garment type.

---

# 1. Kalamkari

### Description
Kalamkari is a traditional Indian textile art that involves **hand-painted or block-printed designs using natural dyes**. It originates primarily from **Andhra Pradesh and Telangana**.

### Visual Characteristics

- Intricate hand-drawn or block printed motifs
- Mythological scenes or storytelling artwork
- Floral vines and temple-inspired elements
- Earthy colors such as red, indigo, mustard, and black
- Fine sketch-like outlines

### Common Uses

- Sarees
- Dupattas
- Wall hangings
- Fabric panels

### Edge Cases

- If the design contains **narrative artwork or mythological illustrations**, classify as `Kalamkari`.
- If the pattern consists only of repeated geometric motifs, it may belong to **Ajrakh** instead.

---

# 2. Ikat

### Description

Ikat is a **resist dyeing technique** where yarns are dyed before weaving to produce characteristic patterns.

### Visual Characteristics

- Slightly blurred or feathered edges in motifs
- Geometric shapes such as diamonds, zigzags, or waves
- Symmetrical repeating patterns
- High color contrast

### Common Uses

- Sarees
- Shawls
- Scarves
- Fabric yardage

### Edge Cases

- If pattern edges appear **blurred due to pre-dyed threads**, classify as `Ikat`.
- Sharp printed motifs typically indicate **Ajrakh** or another block print technique.

---

# 3. Pashmina

### Description

Pashmina refers to **luxurious fine wool textiles** traditionally produced in **Kashmir** using extremely soft cashmere fibers.

### Visual Characteristics

- Soft wool texture
- Subtle woven patterns
- Often plain or minimally patterned
- Elegant embroidery or woven motifs
- Neutral or pastel color palettes

### Common Uses

- Shawls
- Scarves
- Luxury winter garments

### Edge Cases

- If the fabric appears **very fine, soft, and woolen**, classify as `Pashmina`.
- If heavy embroidery dominates the design, verify that the base fabric still resembles **Pashmina wool**.

---

# 4. Ajrakh

### Description

Ajrakh is a traditional **block printing technique** originating from **Kutch (Gujarat) and Sindh regions**.

### Visual Characteristics

- Highly symmetrical geometric patterns
- Deep indigo, red, and black color palette
- Complex star, lattice, and floral motifs
- Dense repeating patterns created using multiple blocks

### Common Uses

- Shawls
- Dupattas
- Fabric panels
- Traditional garments

### Edge Cases

- If the design features **dense geometric symmetry**, classify as `Ajrakh`.
- If motifs depict storytelling scenes rather than geometric patterns, classify as **Kalamkari**.

---

# 5. Chikankari

### Description

Chikankari is a **traditional embroidery technique** from **Lucknow**, known for its delicate threadwork.

### Visual Characteristics

- Fine hand embroidery
- Floral and paisley motifs
- White thread embroidery on light fabrics
- Soft elegant textures
- Pastel fabric backgrounds

### Common Uses

- Kurtis
- Sarees
- Dupattas
- Ethnic dresses

### Edge Cases

- If patterns are **embroidered rather than printed**, classify as `Chikankari`.
- If patterns are woven into the fabric instead of stitched, it likely belongs to another class.

---

# Annotation Guidelines

To maintain consistency across the dataset, the following annotation rules were applied.

### Image Quality Filtering

Images were excluded if they were:

- blurry or low resolution
- heavily edited or filtered
- containing less than **40% visible textile surface**

### Annotation Process

1. Each class was defined using **reference examples and visual guidelines**.
2. The first **100 images were labeled by multiple annotators** to check agreement.
3. Disagreements were discussed and annotation rules were refined.
4. Remaining images were divided among team members for annotation.

### Dataset Focus

The dataset emphasizes **textile patterns rather than garment shapes**, ensuring models learn to recognize **fabric techniques and cultural textile styles**.

---

# Summary

The five classes in the **Bharat Textile Net dataset** represent distinctive Indian textile traditions:

- Kalamkari — narrative hand-painted/block printed textiles
- Ikat — resist-dyed woven patterns
- Pashmina — luxury wool textiles from Kashmir
- Ajrakh — geometric block printed fabrics
- Chikankari — delicate embroidery from Lucknow

These categories allow deep learning models to recognize **fine-grained textile styles unique to Indian cultural heritage**.
