# Ab Initio Structure Prediction of CD8 Alpha Chain

## Author
* **Name:** Şevval Peköz
* **Institution:** Inonu University - Department of Molecular Biology and Genetics
* **Course:** Molecular Modeling

## Project Overview
This project focuses on the *ab initio* structural prediction of the **CD8 alpha (CD8A)** protein using AlphaFold. CD8 is a vital transmembrane glycoprotein found on the surface of cytotoxic T lymphocytes (CTLs). It acts as a co-receptor for the T-cell receptor (TCR), playing a fundamental role in the immune system's ability to recognize and eliminate infected or malignant cells.

The primary biological function of CD8 is to bind specifically to the **alpha-3 (α3) domain of MHC Class I** molecules. This interaction stabilizes the TCR-peptide-MHC complex and facilitates intracellular signaling by recruiting the **Lck kinase** to the T-cell receptor complex, which is essential for T-cell activation and the induction of apoptosis in target cells.

## Methodology
The structural prediction was performed using **AlphaFold**, focusing on a complex consisting of MHC Class I, Beta-2-microglobulin, and the CD8 alpha chain. The following steps were taken for model evaluation:

1.  **Sequence Selection:** The FASTA sequence corresponding to the CD8 alpha chain (Chain D) was utilized.
2.  **Model Generation:** Five independent structural models were generated.
3.  **Confidence Scoring (pLDDT):** Each model was evaluated based on its Predicted Local Distance Difference Test (pLDDT) score, which indicates the per-residue confidence of the prediction.
4.  **Structural Comparison (RMSD):** Pairwise Root Mean Square Deviation (RMSD) was calculated between the models to assess structural convergence. The models showed high similarity, with RMSD values ranging between **0.54 Å and 0.87 Å**.

## Results and Model Selection
Among the five models produced, **Model 0** was selected as the final structure for further analysis.

* **Overall Complex pLDDT:** 89.44
* **CD8A Chain (Chain D) pLDDT:** **81.04** (Highest confidence score)
* **Selection Criteria:** Model 0 demonstrated the highest structural confidence for the CD8A chain specifically, ensuring a reliable representation of the immunoglobulin-like fold of the extracellular domain.

## Files in the Repository
* `fold_2026_04_19_16_51_model_0.cif`: The selected AlphaFold prediction model (Best confidence).
* `cd8_pymol_render.png`: High-resolution render of the CD8A protein structure.
* `README.md`: Project documentation and report.
