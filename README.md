# Machine Learning - Abalone Data Analysis (CA1)

> This project is about analyzing the Abalone dataset using the CRISP-DM framework. The main goal is to use machine learning to predict the physical features of abalones (classification for sex and regression for age). This can help replace the old, slow, and invasive method of cutting the shell and counting the rings under a microscope.

This project was done for Continuous Assessment 1 (CA1) in the **Machine Learning (Level 7)** module for the L7 Dip. in Data Analytics program at CCT College Dublin.
**Student:** Andrii Semeniuk 

## Key Features of the Project

I divided the project into two main machine learning tasks:
* **Classification:** I tried to predict the sex of the abalone (Male, Female, Infant) based on its size and weight. I trained and tested three models: Decision Tree, K-Nearest Neighbors (KNN), and Logistic Regression.
* **Regression:** I tried to predict the age (number of `Rings`) using numerical features. For this, I used Linear Regression, Lasso (L1), and Ridge (L2) algorithms.
* **Methodology:** I strictly followed the **CRISP-DM** standard, from understanding the business problem to evaluating the models.
* **Data Cleaning (EDA):** I explored the original dataset (4177 rows and 9 columns), checked for missing values, and removed duplicates.

## Results and Conclusions

* **Classification:** All three models (Tree, KNN, Logistic Regression) reached a maximum accuracy of about **55%**. When I looked at the Confusion Matrix, I noticed that the models often mixed up females and infants. Conclusion: their shell sizes overlap too much in real life, so it's impossible to separate them perfectly using only physical measurements.
* **Regression:** The models got an $R^2 \approx 0.51$, which means we can explain about half of the variance in age. The Mean Absolute Error (MAE) was around 1.6 rings. The **Ridge (L2)** model worked best for this dataset because our features are highly correlated.

## Tech Stack

* **Programming Language:** Python 3
* **Environment:** Jupyter Notebook
* **Libraries:** * Data handling: `pandas`, `numpy`
    * Visualization: `matplotlib`, `seaborn`
    * Machine Learning (`scikit-learn`): `StandardScaler`, `LogisticRegression`, `KNeighborsClassifier`, `DecisionTreeClassifier`, `LinearRegression`, `Lasso`, `Ridge`

## Repository Structure

* `CA1 Machine Learning.ipynb` — The main Jupyter Notebook with all the code, CRISP-DM steps, and final conclusions.
* `abalone.csv` — The dataset I used to train the models.
* `Data Dictionary - Abalone dataset.docx` — A document explaining what each column in the dataset means.

## How to Run

### 1. Clone the repository:
   ```bash
   git clone https://github.com/SemenyukAndrey/Machine-Learning---Abalone-Dataset-CA1-.git
```
### 2. Install the needed Python libraries if you don't have them yet:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```
### 3. Start Jupyter Notebook in the project folder:
```bash
jupyter notebook
```
### 4. Open the CA1 Machine Learning.ipynb file and run all the cells from top to bottom.

---
## Author
Andrii Semeniuk  
Diploma in Data Analytics for Business, CCT College Dublin
