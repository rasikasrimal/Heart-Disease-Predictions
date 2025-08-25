<!-- Title -->
<p style="background-color:#28334AFF;
          font-family:'Times New Roman', serif;
          font-size:150%;
          text-align:center;
          color:#FFFFFF;
          padding:10px 20px;
          border-radius:15px;">
  Heart Disease Prediction Project Structure
</p>

<!-- Content -->
<div style="border-radius:12px; 
            padding:18px; 
            background-color:#F9F9F9; 
            font-size:115%; 
            line-height:1.6; 
            font-family:'Times New Roman', serif;
            color:#000000;">

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">1. Project Overview</h3>
  <p>
    This project applies <strong>EDA, preprocessing, and machine learning</strong> to the 
    <em>UCI Heart Disease Dataset</em>, focusing on classification using Random Forest 
    and XGBoost. The objective is to detect heart disease with high accuracy by 
    cleaning data, handling outliers, and training robust models.
  </p>
  <ul>
    <li><strong>Objectives:</strong> EDA, preprocessing (missing values, scaling), Random Forest & XGBoost training</li>
    <li><strong>Dataset:</strong> UCI Heart Disease (920 entries, 16 columns)</li>
    <li><strong>Tools:</strong> pandas, numpy, matplotlib, seaborn, plotly, scikit-learn, xgboost</li>
  </ul>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">2. Importing Libraries</h3>
  <p>Libraries for data handling, visualization, preprocessing, modeling, and evaluation.</p>
  <ul>
    <li><strong>Data Handling:</strong> pandas, numpy</li>
    <li><strong>Visualization:</strong> matplotlib, seaborn, plotly</li>
    <li><strong>Preprocessing:</strong> StandardScaler, LabelEncoder, SimpleImputer, KNNImputer, IterativeImputer</li>
    <li><strong>Modeling:</strong> LogisticRegression, KNN, SVC, DecisionTree, RandomForest, AdaBoost, GradientBoost, XGBoost</li>
    <li><strong>Metrics:</strong> accuracy, confusion_matrix, classification_report</li>
  </ul>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">3. Loading the Dataset</h3>
  <p>
    CSV file loaded with <code>pandas</code>. Initial checks: 
    <code>df.head()</code>, <code>df.info()</code>, <code>df.shape()</code>, 
    and min/max value ranges.
  </p>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">4. Exploratory Data Analysis (EDA)</h3>
  <p>
    Distribution analysis, grouped comparisons, and visualization for key variables.
  </p>
  <ul>
    <li><strong>Age:</strong> Histogram, KDE, grouped by sex</li>
    <li><strong>Sex:</strong> Pie charts, bar plots</li>
    <li><strong>Chest Pain (cp):</strong> Value counts, crosstabs, bar plots</li>
    <li><strong>Resting BP, Cholesterol:</strong> Boxplots, histograms</li>
    <li><strong>Thalassemia, Target:</strong> Countplots, grouped analysis</li>
  </ul>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">5. Data Preprocessing</h3>
  <ul>
    <li><strong>Missing Values:</strong> IterativeImputer, RandomForest-based imputation</li>
    <li><strong>Outliers:</strong> Boxplot detection, removed extreme values (trestbps=0)</li>
    <li><strong>Feature Engineering:</strong> Encoded categorical variables, created clean dataset</li>
  </ul>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">6. Model Training & Evaluation</h3>
  <ul>
    <li><strong>Random Forest:</strong> GridSearchCV tuning, accuracy evaluation</li>
    <li><strong>XGBoost:</strong> Hyperparameter tuning, ROC-AUC evaluation</li>
    <li><strong>Target:</strong> Multi-class (0–4) and binary classification (0 vs 1+)</li>
  </ul>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">7. Conclusion & Notes</h3>
  <ul>
    <li><strong>Insights:</strong> Imbalance (male > female), cp and thal highly predictive</li>
    <li><strong>Model Advantages:</strong> RF robust to missing values, XGBoost high accuracy</li>
    <li><strong>Future Work:</strong> More models, feature selection, deployment</li>
  </ul>

  <h3 style="color:#28334AFF; font-size:120%; margin-top:10px;">Appendix: Dataset Columns</h3>
  <table style="width:100%; border-collapse:collapse; font-size:15px; margin-top:10px;">
    <thead>
      <tr style="background-color:#E0E0E0;">
        <th style="border:1px solid #999; padding:6px;">Column</th>
        <th style="border:1px solid #999; padding:6px;">Description</th>
        <th style="border:1px solid #999; padding:6px;">Type</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>age</td><td>Age</td><td>int</td></tr>
      <tr><td>sex</td><td>Male/Female</td><td>object</td></tr>
      <tr><td>cp</td><td>Chest pain type</td><td>object</td></tr>
      <tr><td>trestbps</td><td>Resting BP</td><td>float</td></tr>
      <tr><td>chol</td><td>Cholesterol</td><td>float</td></tr>
      <tr><td>thal</td><td>Thalassemia</td><td>object</td></tr>
      <tr><td>num</td><td>Target (0–4)</td><td>int</td></tr>
    </tbody>
  </table>
</div>
