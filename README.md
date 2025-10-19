# 🚀 CERN Anomaly Detection in Dimuon Events

This project applies machine learning techniques to detect **anomalous dimuon events** in proton-proton collision data recorded at the Large Hadron Collider.  
We use unsupervised algorithms to identify rare, high-energy events that may correspond to interesting or unexpected physical phenomena.

## 📊 Dataset

- 📂 Source: [CERN Open Data Portal](https://opendata.cern.ch/record/545)  
- 🧪 File used: `Dimuon_DoubleMu.csv`  
- 💡 Events recorded by CMS detector at √s = 7 TeV  
- 🧮 Variables:
  - `E1`, `E2` — energy of muon 1 and 2  
  - `pt1`, `pt2` — transverse momentum  
  - `eta1`, `eta2` — pseudorapidity  
  - `phi1`, `phi2` — azimuthal angle  
  - `M` — invariant mass

## 🧠 Methods Used

- **Data Preprocessing**  
  - Standardization with `StandardScaler`  
  - Feature selection and cleaning

- **Anomaly Detection Models**
  - Isolation Forest  
  - Local Outlier Factor

- **Visualization**
  - Scatter plots
  - KDE distributions
  - Pair plots
  - Mass distribution curves


## 🧰 Requirements

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
