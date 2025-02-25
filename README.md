# Nonverbal-Dynamics-VC-Resolution

This repository contains code and data for the paper:

> **C. Diao, S. A. Arboleda, and A. Raake.**  
> Nonverbal Dynamics in Dyadic Videoconferencing Interaction: The Role of Video Resolution and Conversational Quality.  
> *In Proceedings of the 26th International Conference on Multimodal Interaction (ICMI '24)*, Association for Computing Machinery, New York, NY, USA, 387–396.

## 📖 Abstract
This paper explores how video resolution and conversational quality influence nonverbal communication during videoconferencing. We analyzed webcam recordings to extract individual nonverbal cues—including body movements, facial expressions, and gaze behavior—and assessed interpersonal synchrony using windowed lagged cross-correlation. The findings reveal that higher video resolution enhances individual expressiveness but may reduce interpersonal synchrony in body movements, while better conversational quality improves facial expression mimicry.

## 📂 Repository Structure
- `data/`: Raw and processed experimental data.
- `scripts/`: R scripts for statistical analysis.
- `results/`: Outputs and plots.
- `README.md`: Project documentation.

## 📝 Analysis Breakdown
**Pseudo Analysis**  
(pseudo_validation_pipeline.Rmd)  
- Validates whether interpersonal synchrony observed in real dyadic interactions is significantly different from pseudo interactions.
- Compares real vs. pseudo interactions with paired t-tests.

**Individual Analysis**
(individual_analysis_pipeline.Rmd)
- Examines indiviual communication behaviors such as eye gaze ROI, facial expressions AU06 and AU12, and body movements.
- Applys Linear Mixed Models (LMM) to investigate how different resoltion conditions affects individual nonverbal communication behavior.

**Dyadic Level Coordination Analysis**  
(dyadic_level_analysis_pipeline.Rmd)
- Analyzes interpersonal synchrony between two participants in a conversation focusing on mutual gaze, body motion coordination and facial mimicry.
- Utilizes rMEA to quantify interpersonal coordination.

**Citation**
If you use this work, please cite:
```@inproceedings{10.1145/3678957.3685733,
author = {Diao, Chenyao and Arevalo Arboleda, Stephanie and Raake, Alexander},
title = {Nonverbal Dynamics in Dyadic Videoconferencing Interaction: The Role of Video Resolution and Conversational Quality},
year = {2024},
isbn = {9798400704628},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3678957.3685733},
doi = {10.1145/3678957.3685733},
booktitle = {Proceedings of the 26th International Conference on Multimodal Interaction},
pages = {387–396},
numpages = {10},
location = {San Jose, Costa Rica},
series = {ICMI '24}
}
```
