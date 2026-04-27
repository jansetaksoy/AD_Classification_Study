# AD_Classification_Study
Alzheimer's Disease Classification
Binary classification of Alzheimer's Disease using machine learning models on clinical and cognitive features.

Installation
bash
git clone https://github.com/janset/aksoy/alzheimers-classification.git
cd alzheimers-classification
pip install -r requirements.txt
Usage
bash
python alzheimer_classification.py
Output is saved to alzheimers_project_outputs/.

Dataset
2,149 patients with 35 clinical features (demographics, cognitive assessments, lifestyle, medical history).

Methods
Three models compared: Logistic Regression, Random Forest, Gradient Boosting. Two feature sets: Clinical-Cognitive (13 features) vs. Clinical + Risk Factors (31 features). 5-fold cross-validation with stratified train/validation/test split.

Results
Model	Features	Test AUC	Accuracy
Gradient Boosting	Clinical-Cognitive (13)	0.946	95.1%
Random Forest	Clinical-Cognitive (13)	0.944	94.4%
Logistic Regression	Clinical-Cognitive (13)	0.887	86.5%
Top predictive features: MMSE, Functional Assessment, ADL, Memory Complaints, Confusion.

References
Dataset: https://www.kaggle.com/datasets/rabieelkharoua/alzheimers-disease-dataset
