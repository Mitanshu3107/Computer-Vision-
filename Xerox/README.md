# Xerox JBIG2 Compression Bug Analysis

## Practical Overview

This practical analyzes a well-known real-world failure involving the Xerox implementation of the JBIG2 compression standard. JBIG2 is a highly efficient compression method designed for binary document images such as scanned text. However, certain implementations introduced a critical flaw where visually similar characters were incorrectly substituted during compression. The objective of this practical is to experimentally demonstrate how compression techniques can introduce semantic errors in document images while remaining visually acceptable to human observers.

---

## Key Concepts / Techniques

- JBIG2 Document Compression
- Connected Component Analysis
- Pattern Substitution Risk
- Image Similarity Metrics (PSNR, SSIM)
- Edge Detection
- Silent Data Corruption Detection
- Compression Impact on Downstream Tasks
- Entropy and Edge Density Analysis
- Document Image Processing

---

## How It Works

The practical is divided into five experimental analyses to study different aspects of compression-related risks.

### 1. Pattern Substitution Risk

Connected components are extracted from a binary document image to represent individual characters or symbols. Simple shape descriptors such as area and bounding box size are used to measure similarity between components. Similar components are grouped together and replaced with a prototype symbol, simulating how aggressive pattern substitution in compression can merge different characters.

---

### 2. Human-Visible vs Machine-Relevant Differences

Multiple JPEG-compressed versions of a document image are generated using different quality levels. Image quality metrics such as PSNR and SSIM are computed to measure perceptual similarity. Edge detection is applied to analyze how compression affects machine-relevant features even when the image still appears visually acceptable to humans.

---

### 3. Silent Data Corruption Detection

Two versions of the same document image are compared: a lossless version and a lossy compressed version. Pixel-wise difference analysis and thresholding techniques are applied to highlight regions where structural distortions or substitutions may have occurred.

---

### 4. When Compression Breaks a Downstream Task

A simple rule-based character recognition approach is used to classify digits based on geometric properties. The recognizer is tested on both original and heavily compressed images to observe how compression artifacts degrade recognition accuracy and affect automated systems.

---

### 5. Designing a Safe Compression Rule

A heuristic compression decision model is implemented using image entropy and edge density. These metrics help determine whether a document image should be compressed using a lossless method, a high-quality lossy method, or not compressed at all, depending on the structural complexity of the image.

---

## Results

The experiments demonstrate that aggressive compression techniques can introduce structural distortions in document images that may not be easily detectable by human observers. Although perceptual similarity metrics remain high, machine-relevant features such as edges, character shapes, and connected components can be altered. These changes can lead to incorrect symbol substitution and failures in automated document processing systems.

---

## Use Case

Understanding compression-related errors is essential in several industrial and large-scale document processing systems, including:

- **Digital Document Archival Systems** – Ensuring long-term integrity of scanned legal and financial records.
- **Banking and Financial Document Processing** – Preventing corruption in scanned checks and invoices.
- **Government Record Digitization** – Preserving accuracy in digitized legal and administrative documents.
- **Optical Character Recognition (OCR) Pipelines** – Maintaining reliable text extraction from scanned documents.
- **Enterprise Document Management Systems** – Ensuring data integrity in automated document workflows.
- **Automated Data Extraction Systems** – Preventing semantic errors during machine-based document interpretation.

---

## Conclusion

This practical demonstrates how compression algorithms optimized for visual similarity can introduce hidden semantic errors in document images. The Xerox JBIG2 bug serves as a critical example of how pattern substitution can alter document meaning without obvious visual degradation. The analysis highlights the importance of designing compression pipelines that preserve machine-relevant information, particularly in applications where data accuracy and document integrity are essential.
