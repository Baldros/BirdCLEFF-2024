# BirdCLEF 2024 - Bird Species Identification by Sound

## Overview
This repository contains code and resources developed for the **BirdCLEF 2024** Kaggle competition. The goal of the competition is to identify under-studied Indian bird species from continuous audio data, using machine learning techniques. The outcomes aim to assist conservation efforts in the Western Ghats, India, by automating the detection and classification of bird calls.

## Goal of the Competition
Birds are critical indicators of biodiversity changes, but traditional biodiversity surveys are costly and logistically challenging. By leveraging **Passive Acoustic Monitoring (PAM)** and **machine learning**, this competition seeks to:

1. **Identify endemic bird species** of the sky-islands of the Western Ghats.
2. **Detect/classify endangered bird species** with limited training data.
3. **Detect/classify nocturnal bird species**, which are less understood.

The best entries will develop reliable classifiers with limited training data and advance avian biodiversity conservation efforts.

---

## Dataset and Context
The dataset includes soundscape data from the **Western Ghats**, a Global Biodiversity Hotspot, characterized by its extraordinary biodiversity and diverse ecosystems. This region faces significant threats due to habitat modification and climate change, making automated monitoring tools essential for biodiversity assessment.

### Data Characteristics:
- Each audio sample is divided into 5-second windows.
- Each row in the submission format represents a prediction of the presence probability of **182 bird species** for a given window.

---

## Key Dates
- **Start Date:** April 3, 2024
- **Entry Deadline:** June 3, 2024
- **Team Merger Deadline:** June 3, 2024
- **Final Submission Deadline:** June 10, 2024

_All deadlines are at 11:59 PM UTC._

---

## Evaluation
The competition uses a **macro-averaged ROC-AUC** evaluation metric, skipping classes with no true positive labels.

### Submission Format
- Each row corresponds to a 5-second audio window.
- Predict the probability for each of the **182 bird species**.
- Submission file must be named `submission.csv`.

---

## Code Requirements
- **Submission Constraints:**
  - CPU Notebooks only (<= 120 minutes runtime).
  - GPU submissions are disabled.
  - Internet access is disabled during runtime.
- **External Data:** Freely and publicly available external data, including pre-trained models, is allowed.

---

## Repository Structure
```
├── data/                 # Scripts and utilities for data processing
├── models/               # Pre-trained models and custom architectures
├── notebooks/            # Kaggle-compatible notebooks for submission
├── src/                  # Core scripts for feature extraction, training, and inference
├── results/              # Generated predictions and evaluation results
├── README.md             # Project documentation
```

---

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your_username/BirdCLEF2024.git
   cd BirdCLEF2024
   ```

2. **Set up the environment:**
   Create a virtual environment and install dependencies.
   ```bash
   python -m venv env
   source env/bin/activate  # For Windows: env\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Prepare the dataset:**
   Download the dataset from the Kaggle competition page and place it in the `data/` directory.

4. **Run notebooks:**
   Navigate to the `notebooks/` directory and execute the training or inference notebooks.

---

## Contributions
Contributions to this repository are welcome! If you have ideas for improvement or new approaches, feel free to open an issue or submit a pull request.

---

## Acknowledgments
This competition is collaboratively organized by:
- Chemnitz University of Technology
- Google Research
- Indian Institute of Science Education and Research (IISER) Tirupati
- K. Lisa Yang Center for Conservation Bioacoustics at the Cornell Lab of Ornithology
- LifeCLEF
- Xeno-canto

Special thanks to Kaggle for hosting this challenge and providing a platform for collaboration.

---

## License
This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
