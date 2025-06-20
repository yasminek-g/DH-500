# Framing Deception: A Multi-Modal Analysis of Political Deepfake Narratives

Drawing from the Political Deepfake Incident Database (PDID) [1], this project aims to analyze the narrative elements encoded in political deepfakes, the attributes that predict their engagement, and the patterns of their dissemination to understand their impact on the information ecosystem.

## Research Questions
We first investigate the online artifacts themselves, analyzing the narratives embedded in the shared deepfakes:
-   **RQ1:** What are the dominant narrative elements—textually and visually—used in political deepfakes?
-   **RQ2:** Which attributes of a political deepfake predict higher levels of virality and engagement?

We further explore how political deepfakes travel through the information ecosystem and intersect with real-world events:
-   **RQ3:** What are the dissemination patterns of political deepfakes, and how do they correlate with real-world events?

## Repository Structure
This repository is organized to support the research, from data preparation to final analysis.

```bash
project_root
├── code
│   └── analysis
│       ├── 0 - text (descriptive) extraction  
│       ├── 1 - visual extraction               
│       ├── 2 - regression
│       └── 3 - dissemination
├── data
│   ├── descriptive narrative extraction
│   ├── initial data
│   └── visual extraction
├── data preparation
├── docs
├── figures
├── models
├── .gitignore
└── README.md
```

-   **`/code/analysis/`**: Contains the Jupyter notebooks for the core analysis, structured by research question.
    -   `0 - text (descriptive) extraction`: Textual analysis for RQ1.
    -   `1 - visual extraction`: Visual analysis (emotions, objects, symbols) for RQ1.
    -   `2 - regression`: Regression modeling to predict virality for RQ2.
    -   `3 - dissemination`: Time-series analysis of dissemination patterns for RQ3.
-   **`/data preparation/`**: Scripts for preprocessing and cleaning the raw data.
-   **`/data/`**: Contains the raw, intermediate, and final datasets used in the analysis. Due to space constraints, this is not included in the final .zip file. See [Data](#data) for more details.
-   **`/docs/`**: Includes the research paper and appendix.
-   **`/figures/`**: Stores charts, plots, and other figures generated during the analysis.
-   **`/models/`**: Contains saved models, such as the topic model.

## Data
The data is organized into three main directories:
-   **`/data/initial data/`**: Contains the data retrieved from the snapshot of the Political Deepfake Incident Database (PDID), with filterings based on year and type of fake (deepfake). 
-   **`/data/descriptive narrative extraction/`**: Contains the data extracted from the PDID, including text and metadata.
-   **`/data/visual extraction/`**: Contains the visual data added to the PDID, including emotions, objects, and symbols.

The data is stored on Google Drive for easy access and sharing in the same structure as above. Any loose files are left for the sole purpose of being able to run the notebooks. Request access here: [PDID Project Data Access Request](https://drive.google.com/drive/folders/1VQBgzOIEVJfY7qDS1w2F0Gq0UK6l3oKF?usp=drive_link).

## Setup

All notebooks run on Colab, with necessary installations included in the notebooks. 

## References 
[1] C. P. Walker, D. S. Schiff, and K. J. Schiff, "Merging AI Incidents Research with Political Misinformation Research: Introducing the Political Deepfakes Incidents Database," in Proceedings of the AAAI Conference on Artificial Intelligence, vol. 38, no. 21, pp. 23053–23058, Mar. 2024. doi: 10.1609/aaai.v38i21.30349.
