# Matrix Factorization using Singular Value Decomposition (SVD)

## Project Overview
This project demonstrates **Matrix Factorization using Singular Value Decomposition (SVD)** on a small synthetic user-item dataset in **Python (Jupyter Notebook)**.  
SVD is widely used for **recommender systems, dimensionality reduction, and noise reduction**.  
The project decomposes a user-item rating matrix, reconstructs it using top singular values, evaluates the reconstruction, and visualizes the results.

---

## Dataset
- **Synthetic User-Item Rating Matrix**  
  - 5 Users: U1, U2, U3, U4, U5  
  - 5 Items: Item1, Item2, Item3, Item4, Item5  
  - Ratings randomly generated from 1 to 5  
  - Some missing values (NaN) to simulate real-world scenarios  

---

## Project Workflow

1. **Data Generation**  
   - Create a small user-item rating matrix with random ratings and missing values.  

2. **Data Preprocessing**  
   - Fill missing values with the **mean of each item**.  

3. **Matrix Factorization**  
   - Apply **SVD** using `numpy.linalg.svd()` to decompose the matrix into `U`, `Σ`, and `V^T`.  
   - Reconstruct the matrix using the top **k singular values** to capture latent features.  

4. **Evaluation**  
   - Compute **RMSE** and **MAE** to measure reconstruction accuracy.  

5. **Visualization**  
   - Heatmaps of the original and reconstructed matrices.  
   - Singular values plot to show feature importance.  

6. **Conclusion & Insights**  
   - SVD effectively captures latent patterns.  
   - Top k singular values preserve most information while reducing noise.  

---

## How to Run
1. Clone this repository:

```bash
git clone <repository-url>
```
2. **Open the Jupyter Notebook**  
   - Open `SVD_Matrix_Factorization.ipynb` in Jupyter Notebook or JupyterLab.

3. **Install Required Libraries** (if not already installed):

```bash
pip install numpy pandas matplotlib seaborn scikit-learn python-docx
```
4. **Run All Cells in the notebook sequentially.**

  - Step 1: Data Generation

  - Step 2: Data Preprocessing

  - Step 3: SVD Factorization and Reconstruction

  - Step 4: Evaluation Metrics

  - Step 5: Visualization

  - Step 6: Conclusion

5. **Word Report Generation**

   The notebook automatically generates SVD_Project_Report.docx with all results, tables, and plots.
