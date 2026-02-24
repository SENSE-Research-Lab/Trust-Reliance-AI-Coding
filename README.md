# Replication Package

**Paper title:**  
*AI or Ally? Understanding Student Reliance on GitHub Copilot and Human Peers Through Eye Tracking*  


## Overview

This repository contains the replication package for the above paper. It includes all experiment-related data and materials used in the statistical analyses, as well as the post-task survey instrument and participant responses.

The data was collected as part of a controlled **eye-tracking study** investigating how software engineering students interact with **GitHub Copilot** and **human peer assistance** during debugging tasks.

---

## Contents

### 1. `metrics_export.csv`
Contains raw and processed eye-tracking metrics exported from **Tobii Pro Lab** for all participants and tasks.

Includes:
- Fixation count  
- Total fixation time  
- Average fixation duration  
- Task timestamps  
- AOI (Area of Interest) mappings  

---

### 2. `metrics_reliance.csv`
Contains key metrics used to quantify **reliance on the assistance type** (Copilot or human peer).

Includes:
- Behavioral reliance indicators (e.g., Assistance Attention Ratio)  
- Aggregated eye-tracking metrics by assistance condition  

---

### 3. `reliance-questionnaires.csv`
Contains participants’ self-reported responses to Likert-scale questions related to:
- Perceived reliance on AI  
- Trust in AI versus human suggestions  
- Perceived impact of assistance type on performance (e.g., speed, concentration, code quality)

---

### 4. `Survey.pdf`
PDF copy of the post-experiment questionnaire administered after participants completed both assistance conditions.

Includes:
- Demographics  
- Trust and reliance scales  
- Open-ended feedback questions  

---

## Usage Notes

- All data has been **fully de-identified** to preserve participant anonymity.  
- The dataset supports replication of the analyses presented in **Sections IV and V** of the paper.  
- Statistical analyses were conducted using **Python-based data analysis libraries** and **R**.

---

If you have any questions regarding the dataset or replication procedure, please contact the principal author: zohreh.sharafi@polymtl.ca
