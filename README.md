# Morphological Analysis of Palmer Archipelago Penguins

## Project Overview
This project evaluates the physical variations among three penguin species (*Adelie*, *Chinstrap*, and *Gentoo*) using the Palmer Penguins dataset. The goal is to determine if skeletal dimensions (flipper length) and body mass are reliable metrics for species classification.

The project encompasses the entire data lifecycle: from processing "messy" raw field observations to analyzing them.

## Key Findings
- **Hypothesis Supported:** The study confirmed that Gentoo penguins occupy a distinct morphological niche, averaging ~1.3kg heavier than other species.
- **Size Correlation:** A strong positive linear correlation exists between flipper length and body mass across all observed genera.
- **Classification Limits:** While Gentoo penguins are easily identified by size, Adelie and Chinstrap species exhibit significant morphological overlap.

## Data Pipeline
The analysis is driven by a Python-based pipeline (`penguin_morphology_analysis.ipynb`) that performs:
1. **Feature Selection:** Reducing 17 raw metadata columns to 8 core biological variables.
2. **Data Imputation:** Handling missing values via median imputation to maintain sample integrity.
3. **Categorical Standardization:** Cleaning species names and handling missing gender records.
4. **Visualization:** Generating distribution plots and correlation scatter plots using `Seaborn` and `Matplotlib`.

## Repository Structure
- `data/`
    - `penguins_raw.csv`: The original, unprocessed field data (17 columns).
    - `cleaned_penguin_data.csv`: The refined dataset exported after the Python cleaning process.
- `outputs/`
    - `report_visuals.png`: Final visualization showing species distribution and mass-to-flipper correlation.
- `penguin_morphology_analysis.ipynb`: The primary Jupyter Notebook containing the cleaning, EDA, and analysis code.
- `README.md`: Project documentation.

## How to Run
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/kevsvoid/palmer-penguin-morphology.git](https://github.com/kevsvoid/palmer-penguin-morphology.git)
2. **Install dependencies:**
 Ensure you have `pandas`, `seaborn`, and `matplotlib` installed.
3. **Run the Analysis:**
 Open the `.ipynb` file in Jupyter Lab or VS Code and run all cells to regenerate the cleaned CSV and visuals.


---

### References

**Gorman KB, Williams TD, Fraser WR (2014)** Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins (Genus *Pygoscelis*). *PLoS ONE* 9(3): e90081.

**Horst AM, Hill AP, Gorman KB (2020)** *palmerpenguins: Palmer Archipelago (Antarctica) penguin data*.
