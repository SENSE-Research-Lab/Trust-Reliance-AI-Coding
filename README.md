# Replication Package

**Paper title:**  
*AI or Ally? Understanding Student Reliance on GitHub Copilot and Human Peers Through Eye Tracking*  


## Overview

This repository contains the replication package for the above paper. It includes all experiment-related data and materials used in the statistical analyses, as well as the post-task survey instrument and participant responses.

The data was collected as part of a controlled **eye-tracking study** investigating how software engineering students interact with **GitHub Copilot** and **human peer assistance** during debugging tasks.

---

## Contents - Data

### 1. `metrics_export.csv`
Contains raw and processed eye-tracking metrics exported from **Tobii Pro Lab** for all participants and tasks.

Includes:
- Fixation count  
- Total fixation time  
- Average fixation duration  
- Task timestamps  
- AOI (Area of Interest) mappings  

### 2. `metrics_reliance.csv`
Contains key metrics used to quantify **reliance on the assistance type** (Copilot or human peer).

Includes:
- Behavioral reliance indicators (e.g., Assistance Attention Ratio)  
- Aggregated eye-tracking metrics by assistance condition  


### 3. `reliance-questionnaires.csv`
Contains participants’ self-reported responses to Likert-scale questions related to:
- Perceived reliance on AI  
- Trust in AI versus human suggestions  
- Perceived impact of assistance type on performance (e.g., speed, concentration, code quality)


### 4. `Survey.pdf`
PDF copy of the post-experiment questionnaire administered after participants completed both assistance conditions.

Includes:
- Demographics  
- Trust and reliance scales  
- Open-ended feedback questions  


## Usage Notes

- All data has been **fully de-identified** to preserve participant anonymity.  
- The dataset supports replication of the analyses presented in **Sections IV and V** of the paper.  
- Statistical analyses were conducted using **Python-based data analysis libraries** and **R**.

---

## Contents - Task descriptions

### Overview

In this study, each participant completed **six debugging tasks** on the open-source Python project **Glances**  
(https://pypi.org/project/glance/).

The tasks were designed to simulate realistic software debugging and feature-extension scenarios and were performed under two assistance conditions:
1. **GitHub Copilot**
2. **Human peer assistance**

Participants received a **standardized instruction file** before starting the experiment, which was read aloud by the researcher and included guidance on eye-tracker calibration, task timing, and interaction constraints.

### Task Structure

- The experiment consisted of **two task series**, each lasting **15 minutes**.
- Each series contained **three debugging tasks**, for a total of **six tasks**.
- Each task was designed to take approximately **5 minutes**.
- A short break was provided between the two task series.
- Eye-tracker calibration was performed before each series.

#### Task Series 1. GitHub Copilot Assistance

In Task Series 1, participants solved debugging tasks **using GitHub Copilot only**. The researcher was not available for assistance during this phase.

**Tasks included:**
1. Handling edge cases in process status counting (`glances/processes.py`)
2. Enhancing fallback logic with timestamps for IO counters (`glances/processes.py`)
3. Adding a request-limited server method (`serve_limited`) to the XML-RPC server (`glances/server.py`)


#### Task Series 2. Human Peer Assistance

In Task Series 2, participants solved debugging tasks **with the help of a peer developer**. Use of GitHub Copilot or prior chat logs was explicitly prohibited.

**Tasks included:**
1. Adding optional plugin filtering to statistics retrieval (`glances/stats.py`)
2. Improving authentication logging (`glances/server.py`)
3. Implementing plugin-level statistics for enabled and disabled plugins (`glances/stats.py`)


### Target Project and Files

All tasks were performed on the **Glances** codebase and focused on the following files:

- `glances/processes.py`
- `glances/server.py`
- `glances/stats.py`

Participants were instructed to validate their solutions by running:

```bash
python -m glances
```
---

## Contact and More Questions

If you have any questions regarding the dataset or replication procedure, please contact the principal author: zohreh.sharafi@polymtl.ca
