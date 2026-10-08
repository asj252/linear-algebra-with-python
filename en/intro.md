---
description: "Free, open linear algebra textbook with Python: geometry first, full proofs, 11 chapters and 13 hands-on experiments, from vectors to the SVD."
---

# Preface

Linear algebra can be viewed as the study of linear spaces and linear mappings.[^lax] The most typical linear spaces are the finite-dimensional Euclidean spaces with Cartesian coordinates, where linear mappings can be understood through matrix multiplication and appear concretely as rotations, reflections, projections, scalings, shears, and their combinations. These transformations are everywhere in the physical world, computer graphics, statistics, and machine learning, and a first-year university linear algebra course usually starts from them.

For mathematicians, the value of linear algebra lies in this: once a problem can be formulated in the framework of linear algebra, it can often be solved completely. Many central topics fall within this framework, such as differentiation and integration on function spaces. Although infinite-dimensional spaces can only partly reuse the finite-dimensional theory, we still often approximate them by finite-dimensional spaces and obtain reliable approximate results. Nor does linear algebra deal only with linear problems: nonlinear topics such as the interactions between linear mappings and the properties of random matrices are also part of its subject matter, and our understanding of the field is still deepening.

What linear algebra abstracts is nothing more than two basic operations: the addition of vectors and the multiplication of vectors by scalars. Remarkably, on such a slender foundation one can raise grand structures in the Romanesque, Gothic, and Baroque styles; more striking still, it not only provides precise theorems for mathematics and its applications, but also supplies a fitting language in which to state these problems.

[^lax]: Peter D. Lax, *Linear Algebra and Its Applications*, 2nd ed., Wiley, 2007.

## What This Book Aims to Do

*Linear Algebra with Python* tries to strike a balance among four aspects: **geometric intuition**, **algebraic structure**, **computational methods**, and **real-world applications**. We start from geometric pictures of linear mappings, use Python code as a tool for interactive exploration and verification, and then move step by step toward abstract definitions and proofs, in the hope that the body of knowledge readers build follows the natural order of understanding and can also be applied directly to solving problems.

To this end, the book makes several choices that differ from traditional textbooks: it uses code to support computation and provides interactive figures; it uses **0-based indexing** throughout, as is common in computer science and physics, rather than the 1-based indexing customary in mathematics textbooks; it treats Gaussian elimination and the PLU decomposition from a single point of view when solving systems of linear equations; and in the chapters on eigenvalues, inner product spaces, and the singular value decomposition it brings in many examples from data science and quantum mechanics.

## Intended Readers and Prerequisites

This book is suitable for undergraduates in mathematics, physics, computer science, engineering, and related fields; graduate students who need to strengthen their foundations in linear algebra; self-learners with some programming background who want to learn linear algebra systematically; and teachers looking for new ways to teach the subject.

Reading the book requires high-school mathematics (functions, coordinate systems, and basic reasoning) and introductory Python (variables, loops, functions). If your programming background is thin, there is no need to worry: the early chapters introduce the syntax and packages we use as they are needed.

## Teaching Philosophy

**Visualization first, abstraction gradually.** People usually build intuition through visual and spatial perception before raising that intuition to abstract understanding. The book therefore begins with concrete transformations in two and three dimensions, accumulates geometric feeling through interactive figures, and only then introduces general vector spaces and abstract definitions.

**Understanding driven by code.** Code in this book is not an appendix but a tool for understanding concepts: readers can verify the conclusions of theorems with code, observe the effects of transformations through visual experiments, and test whether the theory holds on real data.

**Theory guided by applications.** Important concepts are introduced from concrete problems whenever possible, and theoretical derivations alternate with applied case studies, so that readers always know why a tool is needed.

## Structure of the Book

The book has 11 chapters, with 13 interactive experiments placed after the relevant chapters. Most chapters come with a separate exercise page, where each exercise has an expandable solution and Python verification code.

| Chapter | Topic | Key content | Accompanying experiments |
|---|---|---|---|
| 1 | Sets and mappings | Set operations; injective, surjective, and bijective mappings | — |
| 2 | Vectors | Linear operations, inner products and projections, cross products | — |
| 3 | Linear mappings and matrices | Matrices motivated by rotations, typical 2D and 3D mappings, the geometric meaning of the determinant | Experiment 1: 2D linear transformations; Experiment 2: 3D linear transformations |
| 4 | Abstract linear spaces | Vector space axioms, linear independence and bases, kernel and image, the rank–nullity theorem | Experiment 3: direct sums and tensor products |
| 5 | Block matrices | Block multiplication, block inverses | Experiment 4: four views of matrix multiplication; Experiment 5: covariance matrices |
| 6 | Systems of linear equations | Reduced row echelon form, the geometric structure of solutions, Gaussian elimination | Experiment 6: step-by-step elimination in the PLU decomposition |
| 7 | Determinants | Definition and properties, computation, applications | — |
| 8 | The eigenvalue problem | Similarity and diagonalization, Jordan canonical form, numerical methods | Experiment 7: eigenvalue multiplicity and dynamical systems; Experiment 8: mixing times of Markov chains |
| 9 | Inner product spaces and orthogonal structure | Orthogonal and unitary matrices, Hermitian matrices, quadratic forms and the principal axis theorem | Experiment 9: Gram–Schmidt orthogonalization |
| 10 | Introduction to quantum mechanics | Quantum states, density matrices, quantum measurement, the uncertainty principle | Experiment 10: the Bloch sphere and quantum gates |
| 11 | The singular value decomposition and its applications | Proof of the SVD, matrix norms, PCA, the pseudoinverse, the Schmidt decomposition | Experiment 11: latent semantic analysis; Experiment 12: eigenfaces; Experiment 13: PCA of the Iris dataset |

The order of the chapters deliberately does not begin with systems of linear equations or determinants. Chapters 1–3 first build intuition for sets, vectors, and matrices as transformations; Chapter 4 makes the leap from the concrete to the abstract; Chapters 5–7 build on this foundation to treat block matrices, systems of equations, and determinants; and Chapters 8–11 go deeper into the internal structure of matrices and connect it to contemporary applications such as quantum mechanics and data science.

Some section titles carry a reading-priority mark: **◇ marks optional extensions**, which can be skipped without affecting the main line; **◆ marks advanced material or proofs**, where on a first reading you may grasp the conclusion and come back to the derivation later.

## Comparison with Existing Textbooks

| Feature | This book | Traditional textbooks | 3Blue1Brown | Axler, *Linear Algebra Done Right* |
|---|---|---|---|---|
| Starting point | Linear mappings and geometric intuition | Systems of linear equations / determinants | Linear mappings and geometric intuition | Linear mappings |
| Programming | Deeply integrated Python | Little or none | Used only for animation | None |
| 3D geometry | Introduced early | Later or not emphasized | Limited | Limited |
| Applications | Throughout the book | Mostly supplementary | Few | Mainly theoretical |
| Abstract spaces | From concrete to abstract | Much computation, little abstraction | Mainly concrete geometry | Abstract and rigorous |
| Interactivity | Interactive Jupyter environment | Static | Animated videos | Static |

## Suggested Learning Paths

**Classroom teaching.** A standard one-semester course can cover Chapters 1–8 and selected parts of Chapters 9–11; a two-semester course can cover the whole book and add the experiments and projects.

**Self-study.** Readers who want to build a solid foundation should first read Chapters 1–5 in full and then choose later chapters according to their interests. Readers oriented toward applications can go directly to Chapters 8 and 11 after Chapters 1–3, together with the corresponding experiments. Readers oriented toward theory should read Chapters 1–9 in order before moving on to Chapters 10 and 11.

| Chapters | Estimated study time | Difficulty | Role |
|---|---|---|---|
| 1–3 | 2–3 weeks | ★★☆☆☆ | Core |
| 4–6 | 3–4 weeks | ★★★☆☆ | Core |
| 7–8 | 3–4 weeks | ★★★★☆ | Core |
| 9 | 2 weeks | ★★★★☆ | Core / extension |
| 10–11 | 3–4 weeks | ★★★★★ | Applications |

## Notation and Conventions

The notation used in the book is collected in full in the [Table of Common Notations](EN_Common_Notations.ipynb). Before reading, please note the following points in particular:

- Indices of vectors, matrices, and sums always start from 0, for example "row 0" and "column 2"; $\text{row}_i(\mathbf{A})$ denotes row $i$ and $\text{col}_j(\mathbf{A})$ denotes column $j$.
- Matrices are written in bold uppercase (such as $\mathbf{A}$) and vectors in bold lowercase (such as $\mathbf{v}$); $\mathbf{A}^\top$ is the transpose and $\mathbf{A}^*$ is the conjugate transpose.
- In important formulas such as inner products, projections, and spectral decompositions, we also give the Dirac notation alongside, for example $\mathbf{u}^*\mathbf{v} = \langle\mathbf{u}|\mathbf{v}\rangle$; the inner product is linear in its second argument and conjugate-linear in its first.

## Working Environment

The book is written as Jupyter notebooks (`.ipynb`), with the text in MyST Markdown, and is compiled into a website with Jupyter Book. We recommend the following ways to use it:

- **Local environment**: Miniconda + JupyterLab.
- **Online environments**: GitHub Codespaces, Google Colab, AWS SageMaker Studio Lab, or Binder, with no local installation required.
- **Dependencies**: listed in `requirements.txt` in the repository (`numpy`, `scipy`, `sympy`, `matplotlib`, `plotly`, `ipywidgets`, `scikit-learn`, and others).

For the source files and environment setup, see the book's [GitHub repository](https://github.com/asj252/linear-algebra-with-python).

## After This Book

After reading this book, readers should understand the geometric meaning of the core concepts of linear algebra, be able to implement basic algorithms themselves and analyze their behavior, and be able to apply this framework to fields such as data science (PCA, SVD, least squares), machine learning (recommender systems, matrix factorization), computer graphics (rotations, projections, and other transformations), quantum computing (quantum states and measurement), dynamical systems (difference and differential equations), and network analysis (PageRank).

## Contributing and Feedback

This book is still being revised. If you find errors, have suggestions for improvement, or would like to share applications or further exercises, you are welcome to contact us through the Issues of the GitHub repository.

We believe that combining geometric intuition, theoretical rigor, computational methods, and real-world applications can make linear algebra both easy to understand and genuinely useful. Whether you are a beginner or a practitioner who wants to reorganize your knowledge, we hope this book offers you a new learning experience. Now, let us begin the journey.
