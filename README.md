# Vertical Fragmentation using K-Means Clustering

## 📌 Project Overview

This project demonstrates **Vertical Fragmentation of a Database Relation** using **K-Means Clustering**. Vertical fragmentation is a key concept in **Distributed Database Systems (DDBMS)** where attributes (columns) of a table are grouped into fragments based on how frequently they are accessed together.

In this project, **K-Means clustering** is applied on an **attribute usage matrix** derived from query access patterns to automatically determine optimal vertical fragments.

---

## 🎯 Objectives

* Understand vertical fragmentation in distributed databases
* Model attribute usage using a query–attribute matrix
* Apply K-Means clustering to group related attributes
* Generate optimal vertical fragments for improved query performance

---

## 🧠 Key Concepts Used

* Distributed Database Systems (DDBMS)
* Vertical Fragmentation
* Attribute Affinity
* Query–Attribute Matrix
* K-Means Clustering (Unsupervised ML)

---

## 📂 Project Structure

```
Vertical-Fragmentation-KMeans/
│
├── data/
│   └── ddbss.csv                  # Input dataset (query–attribute matrix)
│
├── notebook/
│   └── Vertical_Fragmentation.ipynb  # Complete implementation
│
├── results/
│   └── fragments.txt              # Output vertical fragments (optional)
│
├── README.md
└── requirements.txt
```

---

## 📊 Dataset Description

* **File:** `ddbss.csv`
* Rows represent **queries**
* Columns represent **attributes**
* Values indicate whether a query accesses a particular attribute

Example:

| Query | A1 | A2 | A3 | A4 |
| ----- | -- | -- | -- | -- |
| Q1    | 1  | 0  | 1  | 0  |
| Q2    | 1  | 1  | 0  | 0  |

---

## ⚙️ Methodology

1. Load query–attribute access matrix
2. Transpose matrix to attribute-centric view
3. Apply **K-Means clustering** on attributes
4. Group attributes based on cluster labels
5. Generate vertical fragments

---

## 🧪 Technologies Used

* Python 3.13
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

## ▶️ How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/Vertical-Fragmentation-KMeans.git

# Navigate to project directory
cd Vertical-Fragmentation-KMeans

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook notebook/Vertical_Fragmentation.ipynb
```

---

## 📈 Output

* Clustered attributes
* Vertical fragments showing grouped attributes
* Improved attribute locality for queries

---

## 🧩 Example Output

```
Fragment 1: A1, A3, A5
Fragment 2: A2, A4
```

---

## 🚀 Future Enhancements

* Compare K-Means with Hierarchical Clustering
* Use cost-based evaluation metrics
* Extend to hybrid (horizontal + vertical) fragmentation

