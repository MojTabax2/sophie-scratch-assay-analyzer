# Soφ Scratch Analyzer: Automated Cell Migration Analysis
*Standardized, multi-layer image analysis for high-throughput scratch assays.*

## Introduction
The **Soφ Scratch Analyzer** is a specialized feature within the [Sophie AI](https://www.clyte.tech/sop-ai) platform designed to eliminate user bias in wound healing (scratch) assays. Unlike manual tools that require subjective parameter setting for every image, Soφ uses a fixed, multi-layer algorithm to ensure every image is analyzed exactly the same way.

## Key Technical Features
* **High Throughput:** Process up to **200 images** in a single batch (100 for Timepoint 1 + 100 for Timepoint 2).
* **Multi-Layer Algorithm:** Combines up to **6 distinct image analysis functions** (edge detection, contrast thresholding, texture analysis, etc.) to accurately identify the cell-free gap.
* **Fixed Parameters:** The analysis parameters remain locked across all images and users, guaranteeing 100% reproducibility.
* **Automated Reporting:** Delivers results directly as an Excel file containing the calculated Gap Area %.

---

## Comparison: Soφ Analyzer vs. ImageJ
Why switch from the standard manual method?

| Feature | ImageJ / Manual Analysis | Soφ Scratch Analyzer |
| :--- | :--- | :--- |
| **Reproducibility** | **Low:** Varies by user and subjective threshold settings. | **Perfect:** Same algorithm applied every time. |
| **Throughput** | **Slow:** Images often processed one by one. | **Fast:** Up to 200 images processed simultaneously. |
| **Accuracy** | **Variable:** Simple thresholding often mistakes debris for cells. | **High:** Multi-layer algorithm distinguishes cells from debris/artifacts. |
| **Output** | Manual data entry into Excel. | Automatic Excel generation. |

---

## Workflow Guide

### Step 1: Prepare Your Data
Ensure your images are organized by time point.
* **Timepoint 1 (T1):** The "0 hour" or initial scratch images (Max 100 images).
* **Timepoint 2 (T2):** The final endpoint images (Max 100 images).
* *Note: Ensure images are clearly labeled for easy matching.*

### Step 2: Upload to Soφ
1.  Navigate to the **Soφ Scratch Analyzer** module on the [Sophie AI Interface](https://www.clyte.tech/sop-ai).
2.  **Upload T1 Set:** Drag and drop your initial batch (up to 100 files).
3.  **Upload T2 Set:** Drag and drop your final batch (up to 100 files).
4.  Confirm the upload count matches your experiment layout.

### Step 3: Automated Analysis
Once uploaded, initiate the analysis.
* **The Process:** Soφ applies its 6-layer algorithm to every image. It standardizes the contrast, detects the scratch edges, filters out floating debris, and calculates the exact pixel area of the gap.
* **No Tuning Needed:** You do *not* need to adjust sliders or threshold values. The system uses a universal standardization method.

### Step 4: Download Results
Upon completion, the system generates a downloadable **Excel (.xlsx)** file.
* **Data Included:**
    * File Name / ID.
    * Gap Area Percentage (%)

---

## Best Practices for Accuracy
To get the best results from the multi-layer algorithm:
1.  **Consistent Lighting:** Ensure your microscope illumination is consistent between T1 and T2.
2.  **Clean Wells:** While Soφ filters debris better than ImageJ, washing wells before imaging improves edge detection.
3.  **Standardized Scratch:** Use a tool like [CytCut](https://www.clyte.tech/product-page/cytcut-wound-healing-assay-tool) to create uniform gaps, making the "Gap Area %" metric more meaningful across replicates.
(Don't worry if your images are not great! Sophie AI is robust enough to hanlde most inputs with consistent accuracy.)

---

*Powered by [CLYTE Technologies](https://www.clyte.tech).*
