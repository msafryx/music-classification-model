# 🎵 Music Genre Classification and Recommender System

This project builds a machine learning model to classify and recommend music genres based on user demographic data such as age and gender. It uses a Decision Tree Classifier to analyze patterns and output genre preferences. The repository includes training scripts, dataset, and a visualization of the decision tree.

---

## 📁 Repository Contents

- `music.csv`: Dataset with user age, gender, and their preferred music genres.
- `music-classification.ipynb`: Jupyter Notebook containing code for loading the data, training the model, and visualizing results.
- `music-recommender.dot`: A Graphviz DOT file that represents the structure of the trained decision tree model.

---

## 📊 Dataset Description

The dataset has the following columns:

- `age`: Age of the user
- `gender`: Gender of the user (0 = Female, 1 = Male)
- `genre`: Preferred music genre (target variable)

Example genres: Acoustic, Classical, Dance, HipHop, Jazz.

---

## 🧠 Model Details

- **Model Used**: Decision Tree Classifier (`sklearn.tree.DecisionTreeClassifier`)
- **Splitting Criterion**: Gini Impurity
- **Target Classes**: 5 music genres
- **Training Approach**: Supervised Learning

The model learns patterns in the dataset to predict which genre a user is likely to prefer based on their age and gender.

---

## 🚀 Getting Started

### 1. Clone the repository:
```bash
git clone https://github.com/your-username/music-recommender.git
cd music-recommender
```

### 2. Install all dependencies from requirements.txt
```bash
pip install -r requirements.txt
```

### (Optional) Install dependencies individually
```bash

pip install pandas scikit-learn matplotlib graphviz
```

### 3. Launch the Jupyter Notebook
```bash
jupyter notebook music-classification.ipynb
```

#### 4. Visualize the decision tree (requires Graphviz installed)
```bash
dot -Tpng music-recommender.dot -o music-tree.png
```
---

Sample Decision Tree

<img width="767" height="455" alt="image" src="https://github.com/user-attachments/assets/f74edcca-a79a-4963-a0e3-fdfc0f4c8c52" />


