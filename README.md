# Impact of Comprehensive Data Preprocessing on Predictive Modelling of COVID-19 Mortality

### Authors: **Sangita Das & Subhrajyoti Maji**

---

## Overview

This repository contains a Jupyter notebook demonstrating the impact of comprehensive data preprocessing on predictive modeling of COVID-19 mortality. The work investigates how structured preprocessing pipelines influence model performance, stability, and reliability across multiple machine learning models.

The study compares a **standard preprocessing pipeline** with a **custom-designed pipeline** that incorporates domain-aware feature construction, computational dependency resolution, and structured outlier handling.

---

## Objectives

- **Explore Computational Dependencies:** Identify and exploit relationships among dataset variables to improve feature consistency and missing value handling.
- **Custom Preprocessing Pipeline:** Develop a structured preprocessing workflow including transformation, correction, and feature refinement steps.
- **Impact Analysis:** Evaluate multiple regression models under different preprocessing regimes and compare performance using RMSE, R², and stability metrics.

---

## Data Source

The dataset is sourced from:

- **Our World in Data (OWID) COVID-19 Dataset**  
  https://github.com/owid/covid-19-data/tree/master/public/data  

Citation:
> Mathieu, E. et al. (2020). *Coronavirus Pandemic (COVID-19)*. OurWorldInData.org.

---

## Repository Contents

- `Enhanced_predictive.ipynb` — Main experimental notebook  
- `data/` — Raw dataset files  
- `standard/` — Outputs from standard preprocessing pipeline  
- `custom/` — Outputs from custom preprocessing pipeline  
- `README.md` — Documentation  
- `LICENSE` — License file  

Both `standard/` and `custom/` directories include:
- trained models  
- processed datasets  
- feature importance tables  
- evaluation results  

---

## Notebook Execution & Display Notes

### ⚠️ Important Rendering Limitation (GitHub + VS Code)

This notebook uses **ipywidgets-based interactive visualisations**.

- On **GitHub**, widget outputs may not render correctly and can show:
  > `Invalid Notebook`

- This is a known limitation of GitHub’s notebook renderer.

- In **VS Code**, widgets may not persist correctly after reopening the notebook:
  - some initial widget-based outputs may not render automatically
  - non-widget outputs (tables, plots, model results) remain fully accessible without re-running

### ✔️ Recommended Usage

To fully experience the notebook:
1. Open in Jupyter Notebook or JupyterLab (or VS Code with active kernel)
2. Run all cells sequentially after opening
3. Ensure `ipywidgets` support is enabled

---

## Installation

```bash
pip install pandas matplotlib seaborn ipywidgets plotly qgrid
```

---

## Notebook Structure

1. Introduction  
2. Setup and Dependencies  
3. Data Preprocessing  
   - Standard pipeline  
   - Custom pipeline  
4. Modeling  
5. Results and Evaluation  
   - RMSE, R², RMSE variance  
6. Conclusion  

---

## Results

The study demonstrates that **comprehensive data preprocessing significantly improves predictive performance and stability**, often exceeding gains obtained from model complexity alone.

Key improvements observed:
- Lower prediction error (RMSE reduction)
- Higher model stability (lower variance across runs)
- Improved feature relevance consistency

---

## Publications

This project has resulted in two research publications:

### 1. Preprint (arXiv)

**Impact of Comprehensive Data Preprocessing on Predictive Modelling of COVID-19 Mortality**  
Das, S., & Maji, S. (2024)  
arXiv preprint: https://arxiv.org/abs/2408.08142  

This work presents the initial experimental findings showing that structured preprocessing pipelines significantly improve predictive performance for COVID-19 mortality modeling.

---

### 2. Journal Publication

**From Raw Data to Reliable Predictions: The Significance of Data Processing in COVID-19 Modelling**  
Das, S., & Maji, S. (2026)  
Asian Journal of Research in Computer Science, 19(2), 75–96  

This work extends the initial study by formalizing the preprocessing framework and demonstrating that data processing quality is a primary determinant of predictive reliability across models.

---

## BibTeX References

```bibtex
@article{das2024impact,
  title={Impact of Comprehensive Data Preprocessing on Predictive Modelling of COVID-19 Mortality},
  author={Das, Sangita and Maji, Subhrajyoti},
  journal={arXiv preprint arXiv:2408.08142},
  year={2024}
}

@article{das2026raw,
  title={From Raw Data to Reliable Predictions: The Significance of Data Processing in COVID-19 Modelling},
  author={Das, Sangita and Maji, Subhrajyoti},
  journal={Asian Journal of Research in Computer Science},
  volume={19},
  number={2},
  pages={75--96},
  year={2026}
}
```

---

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
