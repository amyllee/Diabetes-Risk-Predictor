# 🩺 Diabetes Risk Predictor
This project uses machine learning to **predict an individual’s risk of diabetes** based on lifestyle and health factors from the **Behavioral Risk Factor Surveillance System (BRFSS) 2015 dataset**.  
It provides an interactive interface for users to input their health information and receive a real-time risk prediction.

---

## 🚀 Features
- **Decision Tree Classifier** built with Scikit-learn  
- **Entropy-based splitting** with optimized `max_depth = 8` for balanced generalization  
- **5-fold stratified cross-validation** for model evaluation  
- **F1-score** used to measure prediction accuracy  
- **Matplotlib visualizations** to display feature importance  
- **Interactive user input interface** for real-time prediction

---

## 🧩 Input Format
Users can enter health information to assess diabetes risk:

| Feature | Description | Input Type |
|----------|--------------|------------|
| `HighBP` | High blood pressure | 1 = Yes, 0 = No |
| `HighChol` | High cholesterol | 1 = Yes, 0 = No |
| `BMI` | Body Mass Index | numeric |
| `Smoker` | Smokes cigarettes | 1 = Yes, 0 = No |
| `Stroke` | History of stroke | 1 = Yes, 0 = No |
| `HeartDiseaseorAttack` | Heart disease or heart attack history | 1 = Yes, 0 = No |
| `PhysActivity` | Regular physical activity | 1 = Yes, 0 = No |
| `Fruits` | Eats fruits regularly | 1 = Yes, 0 = No |
| `Veggies` | Eats vegetables regularly | 1 = Yes, 0 = No |
| `HvyAlcoholConsump` | Heavy alcohol consumption | 1 = Yes, 0 = No |
| `AnyHealthcare` | Has healthcare coverage | 1 = Yes, 0 = No |
| `GenHlth` | General health rating | 1–5 (1 = Excellent, 5 = Poor) |
| `PhysHlth` | Number of physically unhealthy days | numeric |
| `Sex` | Biological sex | 0 = Female, 1 = Male |
| `Age` | Age in years | numeric |

**Example Input**
HighBP: 1
HighChol: 0
BMI: 27.3
Smoker: 0
Stroke: 1
HeartDiseaseorAttack: 1
PhysActivity: 1
Fruits: 0
Veggies: 1
HvyAlcoholConsump: 1
AnyHealthcare: 0
GenHlth: 1
PhysHlth: 0
Sex: 1
Age: 45

**Predicted diagnosis:** `No Diabetes`

---

## 📊 Model Performance
- **Model:** Decision Tree Classifier  
- **Criterion:** Entropy  
- **Optimized hyperparameter:** `max_depth = 8`  
- **Cross-validation:** 5-fold stratified  
- **Metric:** F1-score  
- **Key Insight:** Physical health, BMI, and general health were the top predictive features.

---

## 🧰 Technologies Used
- Python  
- Scikit-learn  
- Pandas  
- NumPy  
- Matplotlib  
- Google Colab / Jupyter Notebook  

---

## 🖥️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Diabetes-Risk-Predictor.git

2. Open the notebook in https://colab.research.google.com/ (Google Colab) or Jupyter Notebook
3. Run all cells to train the model, evaluate performance, and enter your own data for real-time prediction

📈 Results:
The model achieved balanced predictive performance and interpretable feature importance, helping users understand which health factors most influence diabetes risk.

👩‍💻 Author:
Amy Lee
Data Science @ University of Michigan
📧 Contact: amyllee@umich.edu