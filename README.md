# Diabetes Prediction Analysis
This project uses a decision tree to predict whether someone might have diabetes, based on common health symptoms like age, weight loss, and vision issues. It shows how machine learning can help identify health risks using a model that's easy to interpret.

---

## Dataset

The dataset includes health-related information collected at the patient level, used to determine the likelihood of a diabetes diagnosis.

- `age`, `gender`
- Symptom indicators such as:
  - `sudden_weight_loss`
  - `visual_blurring`
  - `itching`, `obesity`, etc.
- Target variable: `result` (Positive or Negative for diabetes)

**File used:** `diabetes.csv`

---

## Methodology

### Data Preparation
- Converted categorical variables to dummy/indicator variables
- Split the dataset into 80% training and 20% testing sets

### Modeling
- Trained a **Decision Tree Classifier** to predict diabetes outcome
- Visualized the first 3 layers of the tree
- Evaluated the model using:
  - **Accuracy Score**
  - **Confusion Matrix**
  - **Classification Report**
    - Precision: Measures how many of the positive predictions were actually correct.
    - Recall: Measures how many actual positive cases were correctly identified.
    - F1-Score: The average of precision and recall 

---

## Results

- **Accuracy**: ~89.4%
- **Model**: Decision Tree Classifier

**Insights:**
- Features like sudden weight loss, visual blurring, and obesity were strong indicators
- The model made balanced predictions on both classes
- Tree structure helped visualize key decision paths  

---

## Tools & Libraries

- Python
- `pandas`, `numpy` – data handling
- `scikit-learn` – modeling & evaluation
- `matplotlib` – visualization
- Jupyter Notebook – project development

---

## Key Takeaways

- Decision Trees offer a clear, interpretable way to model binary health outcomes
- Preprocessing categorical data correctly is essential for classification performance
- Visual tools like confusion matrices and tree plots help validate model behavior

---

## Business Implications
**Early Risk Detection**

Helps healthcare providers or wellness programs identify high-risk individuals early, enabling preventative care and lowering long-term treatment costs.

**Cost Reduction**

By catching potential diabetes cases earlier, healthcare systems may avoid more expensive, long-term complications like hospitalization or surgeries.

**Resource Allocation**

Clinics and hospitals can prioritize follow-ups or screenings for patients flagged as high risk, improving efficiency and patient outcomes.
