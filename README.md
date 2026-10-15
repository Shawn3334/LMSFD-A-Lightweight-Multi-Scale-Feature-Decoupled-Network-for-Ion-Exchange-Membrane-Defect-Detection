<div align="center">
  <h1>LMSFD</h1>
  <p><em>A Lightweight Multi-Scale Feature-Decoupled Network for<br>Ion-Exchange Membrane Defect Detection</em></p>
  <p><a href="#im11-det">Dataset</a> · <a href="#detection-results">Results</a> · <a href="#code">Code</a></p>
</div>

LMSFD is a lightweight detector for visual inspection of ion-exchange membranes. It refines spatial and semantic features separately before combining information across scales, targeting small, low-contrast and co-occurring defects.

**IM11-DET:** 1,843 images · 8,514 annotated defects · 11 categories  
**LMSFD:** 87.3% AP<sub>50</sub> · 71.6% AP<sub>50–95</sub> · 10.2M parameters on a held-out production batch

## IM11-DET

Images were collected with a roll-fed line-scan inspection system. Four production batches were used for training and a fifth was held out for validation. The figure shows representative defects, the imaging setup, category counts and defect-size distribution.

<p align="center">
  <a href="datasets.png"><img src="datasets.png" alt="IM11-DET samples, inspection system, and dataset statistics" width="900"></a><br>
  <sub>IM11-DET: representative samples and dataset overview</sub>
</p>

## Detection results

### Quantitative comparison

LMSFD is compared with 11 other detectors on IM11-DET. The right panel shows its gains over the RT-DETR baseline in percentage points.

<p align="center">
  <a href="Comparison.png"><img src="Comparison.png" alt="Comparison of LMSFD with other detectors" width="900"></a><br>
  <sub>Performance across eight detection metrics</sub>
</p>

### Qualitative comparison

Examples from four validation images compare LMSFD with five representative detectors. Orange boxes indicate ground truth; red, yellow and green dashed boxes indicate false positives, false negatives and true positives.

<p align="center">
  <a href="visualization.png"><img src="visualization.png" alt="Qualitative detection comparison on IM11-DET" width="800"></a><br>
  <sub>Detection examples on IM11-DET</sub>
</p>

## Code

The source code will be released after the paper is accepted.
