<div align="center">
  <img src="banner.svg" alt="LMSFD — Ion-exchange membrane defect detection" width="100%" />

  <h1>LMSFD</h1>
  <p><strong>A Lightweight Multi-Scale Feature-Decoupled Network<br />for Ion-Exchange Membrane Defect Detection</strong></p>
  <p>Industrial visual inspection &nbsp;·&nbsp; Multi-scale defects &nbsp;·&nbsp; Lightweight detection</p>
</div>

---

Flexible ion-exchange membranes present low-contrast defects that vary widely in size and often appear together. **LMSFD** separates spatial and semantic feature refinement before cross-scale fusion. This page shares a preview of the **IM11-DET** dataset and selected detection results.

> [!NOTE]
> **Code release:** The source code will be made available after the paper is accepted.

## At a glance

| IM11-DET | Evaluation | LMSFD on the held-out batch |
| :---: | :---: | :---: |
| **1,843** images · **8,514** instances<br />**11** defect categories | **4** production batches for training<br />**1** batch held out for validation | **87.3%** AP<sub>50</sub> · **71.6%** AP<sub>50–95</sub><br />**10.2M** parameters |

## Figures

### 01 &nbsp; Dataset and imaging system

Six representative samples, the roll-fed line-scan setup, category-wise instance counts, and defect-size distribution in IM11-DET.

[![IM11-DET dataset and imaging system](datasets.png)](datasets.png)

<p align="center"><sub>Figure 1 · IM11-DET dataset overview. Click to view at full resolution.</sub></p>

### 02 &nbsp; Quantitative comparison

LMSFD is compared with 11 other detectors across eight metrics. The radar plot normalizes each metric across methods; the right panel shows gains over the RT-DETR baseline in percentage points.

[![Detection performance comparison on IM11-DET](Comparison.png)](Comparison.png)

<p align="center"><sub>Figure 2 · Performance comparison on IM11-DET. Click to view at full resolution.</sub></p>

### 03 &nbsp; Qualitative comparison

Predictions from LMSFD and five representative detectors on four IM11-DET images. Orange solid boxes mark ground truth; red, yellow, and green dashed boxes mark false positives, false negatives, and true positives, respectively.

[![Qualitative detection comparison on IM11-DET](visualization.png)](visualization.png)

<p align="center"><sub>Figure 3 · Detection examples. Click to view at full resolution.</sub></p>
