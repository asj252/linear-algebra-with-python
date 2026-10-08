# Linear Algebra with Python

An interactive linear algebra textbook written as Jupyter notebooks. It starts from the geometry of linear mappings, develops the theory with full proofs, and uses Python throughout for computation, verification, and interactive figures — from vectors and matrices to the singular value decomposition, with applications in data science and quantum mechanics.

**Read online:** https://asj252.github.io/linear-algebra-with-python/

This repository currently contains the **English edition** (`en/`). Traditional and Simplified Chinese editions will be added later.

## Authors

An-Sheng Jhang and Ping-Zen Ong

## Running the notebooks

Every notebook can be run in the browser without installing anything:

- **Google Colab**: use the Colab links in the table below (a Google account is required).
- **Binder**: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/asj252/linear-algebra-with-python/HEAD) — starts JupyterLab with all dependencies; the first launch can take a few minutes.

To run locally:

```bash
git clone https://github.com/asj252/linear-algebra-with-python.git
cd linear-algebra-with-python
pip install -r requirements.txt jupyterlab
jupyter lab
```

The interactive figures use Plotly `FigureWidget` and ipywidgets, which work best in JupyterLab. The read-online site shows the text, code and saved output; the sliders need a live Jupyter kernel, so use Colab, Binder or a local JupyterLab for those.

## Contents

- [Table of Common Notations](https://asj252.github.io/linear-algebra-with-python/en/en-common-notations) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Common_Notations.ipynb)
- [Chapter 1 Sets and Mappings](https://asj252.github.io/linear-algebra-with-python/en/en-chap1-set) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap1_Set.ipynb)
- [Chapter 2 Vectors](https://asj252.github.io/linear-algebra-with-python/en/en-chap2-vector) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap2_Vector.ipynb)
  - [Chapter 2 Vectors: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap2-vector-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap2_Vector_Exercises.ipynb)
- [Chapter 3 Linear Mappings and Matrices](https://asj252.github.io/linear-algebra-with-python/en/en-chap3-linear-transformation-matrix) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap3_Linear_Transformation_Matrix.ipynb)
  - [Chapter 3 Linear Mappings and Matrices: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap3-linear-transformation-matrix-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap3_Linear_Transformation_Matrix_Exercises.ipynb)
  - [Chapter 3 Experiment 1: Two-Dimensional Linear Transformations and Interactive Visualization](https://asj252.github.io/linear-algebra-with-python/en/en-exp1-2d-linear) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP1_2D_Linear.ipynb)
  - [Chapter 3 Experiment 2: Visualizing Three-Dimensional Linear Transformations](https://asj252.github.io/linear-algebra-with-python/en/en-exp2-3d-linear) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP2_3D_Linear.ipynb)
- [Chapter 4 Abstract Linear Spaces](https://asj252.github.io/linear-algebra-with-python/en/en-chap4-abstract-linear-space) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap4_Abstract_Linear_Space.ipynb)
  - [Chapter 4 Abstract Linear Spaces: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap4-abstract-linear-space-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap4_Abstract_Linear_Space_Exercises.ipynb)
  - [Chapter 4 Experiment 3: Direct Sums and Tensor Products as Data Structures](https://asj252.github.io/linear-algebra-with-python/en/en-exp3-tensor-product) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP3_Tensor_Product.ipynb)
- [Chapter 5 Block Matrices](https://asj252.github.io/linear-algebra-with-python/en/en-chap5-block-matrix) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap5_Block_Matrix.ipynb)
  - [Chapter 5 Block Matrices: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap5-block-matrix-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap5_Block_Matrix_Exercises.ipynb)
  - [Chapter 5 Experiment 4: Four Views of Matrix Multiplication](https://asj252.github.io/linear-algebra-with-python/en/en-exp4-block) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP4_Block.ipynb)
  - [Chapter 5 Experiment 5: Covariance Matrices and Block Matrix Operations](https://asj252.github.io/linear-algebra-with-python/en/en-exp5-covariance) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP5_Covariance.ipynb)
- [Chapter 6 Systems of Linear Equations](https://asj252.github.io/linear-algebra-with-python/en/en-chap6-linear-system) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap6_Linear_System.ipynb)
  - [Chapter 6 Systems of Linear Equations: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap6-linear-system-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap6_Linear_System_Exercises.ipynb)
  - [Chapter 6 Experiment 6: Step-by-Step Elimination in Gaussian Elimination/PLU Decomposition and the Rank-One View](https://asj252.github.io/linear-algebra-with-python/en/en-exp6-plu) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP6_PLU.ipynb)
- [Chapter 7 Determinants](https://asj252.github.io/linear-algebra-with-python/en/en-chap7-determinant) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap7_Determinant.ipynb)
  - [Chapter 7 Determinants: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap7-determinant-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap7_Determinant_Exercises.ipynb)
- [Chapter 8 The Eigenvalue Problem](https://asj252.github.io/linear-algebra-with-python/en/en-chap8-eigenvalue-problem) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap8_Eigenvalue_Problem.ipynb)
  - [Chapter 8 The Eigenvalue Problem: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap8-eigenvalue-problem-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap8_Eigenvalue_Problem_Exercises.ipynb)
  - [Chapter 8 Experiment 7: Eigenvalue Multiplicity and Dynamical Systems](https://asj252.github.io/linear-algebra-with-python/en/en-exp7-eigenvalue-multiplicity) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP7_Eigenvalue_Multiplicity.ipynb)
  - [Chapter 8 Experiment 8: Mixing Times of Markov Chains and Matrix Structure](https://asj252.github.io/linear-algebra-with-python/en/en-exp8-markov) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP8_Markov.ipynb)
- [Chapter 9 Inner Product Spaces and Orthogonal Structure](https://asj252.github.io/linear-algebra-with-python/en/en-chap9-inner-product-space) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap9_Inner_Product_Space.ipynb)
  - [Chapter 9 Inner Product Spaces and Orthogonal Structure: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap9-inner-product-space-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap9_Inner_Product_Space_Exercises.ipynb)
  - [Chapter 9 Experiment 9: Visualizing the Steps of Gram-Schmidt Orthogonalization](https://asj252.github.io/linear-algebra-with-python/en/en-exp9-gramschmidt) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP9_GramSchmidt.ipynb)
- [Chapter 10 ◆ Introduction to Quantum Mechanics](https://asj252.github.io/linear-algebra-with-python/en/en-chap10-quantum-physics) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap10_Quantum_Physics.ipynb)
  - [Chapter 10 ◆ Introduction to Quantum Mechanics: Exercises](https://asj252.github.io/linear-algebra-with-python/en/en-chap10-quantum-physics-exercises) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap10_Quantum_Physics_Exercises.ipynb)
  - [Chapter 10 Experiment 10: The Bloch Sphere, Quantum Gates, and the Uncertainty Principle](https://asj252.github.io/linear-algebra-with-python/en/en-exp10-bloch-sphere) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP10_Bloch_Sphere.ipynb)
- [Chapter 11 Singular Value Decomposition and Its Applications](https://asj252.github.io/linear-algebra-with-python/en/en-chap11-singular-value-decomposition) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_Chap11_Singular_Value_Decomposition.ipynb)
  - [Chapter 11 Experiment 11: Latent Semantic Analysis (LSA) and the SVD](https://asj252.github.io/linear-algebra-with-python/en/en-exp11-lsa) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP11_LSA.ipynb)
  - [Chapter 11 Experiment 12: ◆ Eigenfaces—Using the SVD to "Understand" Faces](https://asj252.github.io/linear-algebra-with-python/en/en-exp12-eigenfaces) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP12_Eigenfaces.ipynb)
  - [Chapter 11 Experiment 13: Principal Component Analysis of the Iris Dataset (Iris PCA)](https://asj252.github.io/linear-algebra-with-python/en/en-exp13-iris-pca) · [Colab](https://colab.research.google.com/github/asj252/linear-algebra-with-python/blob/main/en/EN_EXP13_Iris_PCA.ipynb)

Sections marked ◇ are optional extensions; sections marked ◆ contain advanced material or proofs.

## Feedback

The book is still being revised. Corrections, suggestions, and examples of how you use it are welcome in [Issues](https://github.com/asj252/linear-algebra-with-python/issues).

## License

- The text and figures of the book are licensed under [CC BY-NC-SA 4.0](LICENSE).
- The code in the notebooks is licensed under the [MIT License](LICENSE-CODE).
