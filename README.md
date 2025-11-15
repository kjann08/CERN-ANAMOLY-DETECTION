# 🚀 CERN Anomaly Detection in Dimuon Events

# 🚀 Anomaly Detection in Proton–Proton Collision Data (CERN Open Data)

This project applies **unsupervised machine learning** to detect anomalous **dimuon events** in real proton–proton collision data recorded at the **CMS detector** at CERN’s Large Hadron Collider (LHC).  
The goal is to identify rare or unusual events that could correspond to detector noise, reconstruction errors, or **potential new physics signals**.

---

## 📊 Dataset

**Source:** CERN Open Data Portal  
**Detector:** CMS  
**Collision Energy:** √s = 7 TeV  

**File Used:** `Dimuon_DoubleMu.csv`

### 🔧 Features in Dataset
- `E1`, `E2` — energies of muon 1 and 2  
- `pt1`, `pt2` — transverse momenta  
- `eta1`, `eta2` — pseudorapidities  
- `phi1`, `phi2` — azimuthal angles  
- `M` — invariant mass (key physics variable)

## 🧠 Objective
To detect **outliers** in dimuon collision events using:
- **Isolation Forest**
- **Local Outlier Factor (LOF)**

These anomalies may correspond to:
- Rare high-mass dimuon events  
- Unusual kinematic configurations  
- Potential signals of physics beyond the Standard Model  

## 🛠 Methods Used

### ✔ 1. Data Preprocessing
- Loaded & cleaned event data  
- Standardized numerical features using `StandardScaler`  
- Removed extreme detector artifacts  
- Explored distributions of physics variables  

### ✔ 2. Anomaly Detection Models
- **Isolation Forest** (tree-based isolation algorithm)  
- **Local Outlier Factor** (density-based anomaly detection)  

### ✔ 3. Visualizations
- Pairplots & event-space structure  
- Mass distribution curves  
- Energy vs momentum scatter plots  
- Anomaly vs normal event comparison  


## 📈 Results
- Identified clusters of anomalous dimuon events  
- Visualized anomalies in invariant mass and transverse momentum  
- Observed deviations that may represent rare high-mass events  

## 🧰 Requirements

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
