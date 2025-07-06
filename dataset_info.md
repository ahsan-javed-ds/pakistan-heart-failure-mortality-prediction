# Dataset Information

## Overview
This dataset contains comprehensive cardiac patient information for heart failure mortality prediction from Pakistani patients, collected by the Computer-Human Interaction and Social Experience Lab (CHISEL) at LUMS University.

**Source**: Open Data Pakistan - Heart Failure Prediction Dataset  
**URL**: https://opendata.com.pk/dataset/the-heart-failure-prediction-pakistan  
**Total Records**: 368 patients  
**Total Features**: 60 (59 features + 1 target variable)

## Feature Categories & Descriptions

### 🧑‍⚕️ **Demographics (5 features)**
- **Age**: Patient's age in years
- **Age.Group**: Categorized age ranges (21-30, 31-40, 41-50, 51-60, 61-70, 71-80)
- **Gender**: Patient's biological sex (Male/Female)
- **Locality**: Geographic location type (Urban/Rural)
- **Marital status**: Patient's marital status (Married/Single/Widowed)

### 🏥 **Medical History & Conditions (10 features)**
- **Life.Style**: Lifestyle factors and habits (free text)
- **Sleep**: Sleep pattern abnormalities (Yes/No)
- **Category**: Customer Billing Type (Free/Paid)
- **Depression**: Clinical depression diagnosis (Yes/No)
- **Hyperlipi**: Hyperlipidemia diagnosis (Yes/No)
- **Smoking**: Smoking habit (Yes/No)
- **Family.History**: Family history of heart disease (Yes/No)
- **F.History**: Binary family history indicator (0/1)
- **Diabetes**: Diabetes mellitus diagnosis (0/1)
- **HTN**: Hypertension diagnosis (Yes/No)
- **Allergies**: Known allergies (Yes/No)

### 🩺 **Vital Signs & Basic Measurements (3 features)**
- **BP**: Blood pressure measurement (mmHg)
- **Thrombolysis**: Thrombolytic therapy received (0/1)
- **BGR**: Blood glucose random (mg/dL)

### 🧪 **Laboratory Tests (19 features)**

#### Kidney Function Tests
- **B.Urea**: Blood urea nitrogen (mg/dL)
- **S.Cr**: Serum creatinine level (mg/dL) - Key kidney function marker
- **S.Sodium**: Serum sodium concentration (mEq/L)
- **S.Potassium**: Serum potassium level (mEq/L)
- **S.Chloride**: Serum chloride level (mEq/L)

#### Cardiac Enzymes
- **C.P.K**: Creatine phosphokinase enzyme level (U/L) - Heart damage marker
- **CK.MB**: Creatine kinase MB fraction (U/L) - Heart-specific enzyme

#### Complete Blood Count (CBC)
- **ESR**: Erythrocyte sedimentation rate (mm/hr) - Inflammation marker
- **WBC**: White blood cell count (cells/μL)
- **RBC**: Red blood cell count (million cells/μL)
- **Hemoglobin**: Hemoglobin concentration (g/dL)
- **P.C.V**: Packed cell volume/Hematocrit (%)
- **M.C.V**: Mean corpuscular volume (fL)
- **M.C.H**: Mean corpuscular hemoglobin (pg)
- **M.C.H.C**: Mean corpuscular hemoglobin concentration (g/dL)
- **PLATELET_COUNT**: Platelet count (cells/μL)

#### Differential Blood Count
- **NEUTROPHIL**: Neutrophil percentage (%)
- **LYMPHO**: Lymphocyte percentage (%)
- **MONOCYTE**: Monocyte percentage (%)
- **EOSINO**: Eosinophil count (cells/μL)

### 📝 **Clinical Notes (3 features)**
- **Others**: Additional clinical findings (free text)
- **CO**: Chief complaints (free text)
- **Diagnosis**: Primary medical diagnosis (free text)

### 🫀 **Cardiac Assessment & Testing (13 features)**
- **Hypersensitivity**: Drug/substance hypersensitivity (Yes/No)
- **cp**: Chest pain type (1-4 scale)
- **trestbps**: Resting blood pressure (mmHg)
- **chol**: Cholesterol level (mg/dL)
- **fbs**: Fasting blood sugar >120 mg/dL (0/1)
- **restecg**: Resting ECG results (0-2 scale)
- **thalach**: Maximum heart rate achieved (bpm)
- **exang**: Exercise-induced angina (0/1)
- **oldpeak**: ST depression induced by exercise (mm)
- **slope**: Peak exercise ST segment slope (1-3)
- **ca**: Number of major vessels colored by fluoroscopy (0-3)
- **thal**: Thalassemia type (3=normal, 6=fixed defect, 7=reversible)
- **num**: Number of heart disease indicators (1-4)

### 💊 **Treatment & Monitoring (4 features)**
- **SK**: Streptokinase treatment (0/1)
- **SK.React**: Streptokinase reaction (Yes/No)
- **Reaction**: Treatment reaction indicator (0/1)
- **Follow.Up**: Follow-up period in days

### 🎯 **Target Variable (1 feature)**
- **Mortality**: Patient mortality outcome (0=Alive, 1=Deceased)

## Key Dataset Characteristics

### Class Distribution
- **Alive (0)**: 288 patients (78.26%)
- **Deceased (1)**: 80 patients (21.74%)
- **Imbalance Ratio**: ~3.6:1 (Class imbalance present)

### Data Quality
- **Missing Values**: None (complete dataset)
- **Data Types**: Mixed (numerical, categorical, free-text)
- **Feature Complexity**: Ranges from simple binary indicators to complex clinical measurements

### Clinical Relevance
This dataset represents a comprehensive cardiac patient assessment including:
- Complete demographic profiling
- Extensive laboratory workup
- Advanced cardiac testing (ECG, stress tests, angiography)
- Treatment history and outcomes
- Follow-up monitoring

### Usage Notes
- **High-cardinality features** (Life.Style, Others, CO, Diagnosis) contain free-text entries
- **Binary encoding**: Some features use 0/1 while others use YES/NO
- **Multiple blood pressure readings** are present (BP, trestbps)
- **Cardiac enzymes** (CPK, CK-MB) are critical for heart attack detection
- **Kidney function markers** (S.Cr, B.Urea) are important for prognosis

This dataset provides an excellent foundation for developing predictive models for heart failure mortality in the Pakistani population, with comprehensive clinical features spanning demographics, laboratory results, and advanced cardiac assessments.
