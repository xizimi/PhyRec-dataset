# PhyRec Dataset

**PhyRec Dataset** is a multimodal dataset specifically designed for contact and remote photoplethysmography (PPG) research. It provides synchronized recordings to facilitate the study of physiological signal extraction and the comparison between pulse wave dynamics and respiratory signals.

## Dataset Overview

The dataset consists of recordings from **17 subjects** (10 male and 7 female, average age: 23 years). Data was collected under two distinct respiratory conditions:
- **Spontaneous Breathing:** Natural, unguided breathing.
- **Controlled Breathing:** Breathing paced by a metronome.

### Acquisition Specifications

| Modality | Device / Source | Resolution / Rate | Format |
| :--- | :--- | :--- | :--- |
| **Video** | Intel RealSense D455 | 640 × 480 @ 30 fps | `.avi` |
| **PPG Signal** | Custom/Commercial Device | 50 Hz | `.npy` |
| **Respiration** | Respiratory Belt | 50 Hz | `.npy` |
| **Lighting** | Auxiliary Light Source | 820 lux (Stable) | - |

> **Note:** All modalities are precisely temporally synchronized.

---

## File Structure & Content

The dataset is organized by Subject ID and Session ID. Each session folder contains synchronized video and signal files.

**Directory Hierarchy:**
```text
/PhyRec/
├── 202412/ (Date)
│   ├── 1734441203/ (Session ID)
│   │   ├── front_Video-0.avi       # Facial video (Front view)
│   │   ├── right_Video-0.avi       # Facial video (Right view)
│   │   ├── up_Video-0.avi          # Facial video (Top view)
│   │   ├── hands_Color.avi         # Hand video (if applicable)
│   │   ├── Serial-COM4_sig.npy     # Contact PPG signal
│   │   ├── Respi-COM5_sig.npy      # Respiratory belt signal
│   │   ├── Serial-COM4_ts.npy      # Timestamps for PPG
│   │   └── ...
```

## Usage Policy

This dataset is intended for research purposes only. Users are required to submit a request form to access the dataset, providing a brief description of their intended research.

### How to Access

1. **Fill out the request form**: To access the dataset, please fill out the [EULA](./End_User_License_Agreement.pdf), detailing your research goals and planned use.
2. **Approval**: After reviewing your request, access will be granted along with a download link.
3. **Attribution**: Please cite the following reference if you use this dataset in your research:

   **Citation**: [Insert citation information here]


## Contact

For any questions or support regarding the dataset, please contact:  
enchfu@njust.edu.cn
