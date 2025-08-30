# 🎯 Tic-Tac-Toe Outcome Prediction

## 📌 Overview
This project predicts whether **Player X wins** a given Tic-Tac-Toe game configuration using a **Decision Tree Classifier** implemented from scratch.  
The model learns from all possible end-game board states and classifies each configuration as:
- **positive** → X wins
- **negative** → X does not win

This project demonstrates:
- Manual implementation of **Entropy & Information Gain**
- Building a **custom Decision Tree**
- Evaluating model performance with **Accuracy** and **Classification Report**

---

## 📊 Dataset
We use the **Tic-Tac-Toe Endgame Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/101/tic%2Btac%2Btoe%2Bendgame).

- **Instances:** 958  
- **Attributes:** 9 categorical (board positions)  
- **Class:** `positive` or `negative`  

Each cell is encoded as:
- `x` → 1  
- `o` → -1  
- `b` → 0 (blank)

---

## ⚙️ Technologies Used
- **Python** 🐍
- **NumPy** & **Pandas** for data handling
- **Scikit-learn** for train-test split and metrics
- **Math & Collections** for entropy calculation and counting

---

## 🧠 Project Workflow
1. **Load Dataset**  
   - `pandas.read_csv()` to load data  
   - Encode categorical values into numeric form

2. **Train-Test Split**  
   - 80% Training, 20% Testing (`train_test_split`)

3. **Implement Decision Tree**  
   - Custom class with entropy & information gain  
   - Recursively split nodes to build tree

4. **Model Training & Prediction**  
   - `fit()` to train model  
   - `predict()` for test data

5. **Evaluation**  
   - Accuracy Score  
   - Precision, Recall, F1-Score (Classification Report)

---

## 🖥️ How to Run
1. **Clone this repository**
```bash
git clone https://github.com/your-username/tic-tac-toe-outcome-prediction.git
cd tic-tac-toe-outcome-prediction
