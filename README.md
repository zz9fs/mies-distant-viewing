# The Skin and the Bone: A Distant Viewing of Miesian Modernism

## Abstract
This project conducts a "Distant Viewing" of the architectural legacy of Ludwig Mies van der Rohe. By shifting the site of inquiry from physical buildings to pixel-based "digital surrogates," this research performs a forensic audit of archival infrastructure. Using the **Distant Viewing Toolkit (DVT)**, it compares a curated cohort from the Ezra Stoller archive (JSTOR) against uncurated web-scraped imagery (Kaggle) to uncover the "Institutional Gaze."

## Key Findings
* **Algorithmic Blindness:** Documented the failure of state-of-the-art object detection (YOLO) to recognize Miesian syntax, often identifying "chairs" while remaining blind to structural "I-beams."
* **The Stoller Signature:** Quantified institutional curation as a form of signal processing, characterized by low visual entropy, geometric discipline (standardized aspect ratios), and optimized tonal ranges.
* **The Metadata Bridge:** Demonstrated that machine numeracy requires humanistic context to "see" history, turning technical failures into successful forensic audits.

## Repository Structure
Based on the project development lifecycle, the repository is organized as follows:

```text
mies-distant-viewing/
├── data/                         # Directory for image assets
├── metadata/                     # The "Metadata Bridge" (17-column CSV)
├── results/                      # Computational outputs and saved plots
├── photo_scrapping.ipynb         # Exploratory script for web-acquisition (access audit)
├── image_exploration.ipynb       # Main analysis script (Entropy, PCA, and DVT)
├── beautiful_soup.ipynb          # Scraping script for the Kaggle "Wild Stratum"
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation

```

## Methodology

### 1. Data Archaeology
The project excavates two "digital strata":
* **The Institutional Stratum:** 74 high-resolution images by Ezra Stoller from JSTOR.
* **The Wild Stratum:** 74 images from the Kaggle "Architectural Styles" dataset.

### 2. The Labor of the Machine (Technical Hurdles)
The scripts in this repository reflect the iterative and often resistant nature of digital humanities work:
* **Acquisition Challenges:** The `photo_scrapping` notebook documents the attempts to download images directly from architectural sites, serving as a forensic record of access denials and institutional boundaries.
* **The "Deep Parse":** The `image_exploration` notebook contains the core logic for the project, including the manual cleaning of 17 metadata columns to create the relational "Metadata Bridge."

## Technical Requirements
To replicate the analysis, ensure the following Python libraries are installed:
* `dvt` (Distant Viewing Toolkit)
* `beautifulsoup4`
* `pandas`
* `matplotlib`
* `scikit-learn` (for PCA)
* `seaborn`

```bash
pip install -r requirements.txt
