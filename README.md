# ⚖️ VerdictAI

## 🧠 Indian Penal Code (IPC) Sections Predictor

A machine learning project that predicts the most suitable **IPC Section**, **description**, and **punishment** based on a user-provided offense text (e.g., *murder*, *theft*, *bribery*). This helps automate the identification of applicable sections from the Indian Penal Code.

---

## 📂 Project Structure

- `IPC.ipynb`: Main Jupyter Notebook containing data preprocessing, model training, and prediction logic.

---

## 🔧 Requirements

Ensure the following are installed:

- Python 3.x  
- NumPy  
- scikit-learn  
- pandas  
- Jupyter Notebook  
- Kaggle IPC dataset  

To install the libraries:



---

## 📥 Data Preparation

1. Download the **Indian Penal Code (IPC) Sections Information** dataset from [Kaggle](https://www.kaggle.com/).
2. Create a folder named `dataset/` in your project root.
3. Place the downloaded dataset file inside the `dataset/` directory.
4. Open the `IPC.ipynb` notebook in Jupyter and run each cell step-by-step to:
   - 🔹 Preprocess the data  
   - 🔹 Train the model  
   - 🔹 Evaluate the results  
   - 🔹 Make predictions on new offenses  

> 💡 Make sure the dataset contains key fields like `Offense`, `Description`, `Punishment`, and `IPC_Section`.

---

---

## 🧠 Model Architecture

Though named a neural network project, this implementation uses **logistic regression classifiers** in combination with **TF-IDF vectorization** to process and classify offense descriptions.

The model predicts three key legal aspects based on input:

- 📝 **Description** – Legal definition of the offense  
- ⚖️ **Punishment** – The penalty prescribed by law  
- 📘 **IPC Section** – Relevant Indian Penal Code section number  

Each classifier is trained **independently** to predict one of the above.

### 🔬 Layers Overview

- 🟢 **Input Layer**: Offense text vectorized using TF-IDF  
- 🟡 **Hidden Layers**: Includes optional dropout for future extension  
- 🔴 **Output Layer**: Softmax classifier for label prediction

---

## 🚀 Usage

### 🔧 Run the Notebook

To start the project:

```bash
jupyter notebook IPC.ipynb



