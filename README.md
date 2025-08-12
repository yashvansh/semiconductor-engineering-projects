# 🏭 Semiconductor Process Optimization & Reliability Projects

This repository contains two projects simulating **data-driven approaches** for improving yield and reliability in semiconductor manufacturing.  
They showcase **Statistical Process Control (SPC)**, **Design of Experiments (DOE)**, **Failure Modes & Effects Analysis (FMEA)**, and **Reliability Modeling**.

---

## 📂 Project 1 — SPC & DOE Optimization

### 📌 Objective
Identify and optimize semiconductor assembly process parameters to improve **yield** and **reduce defects**.

### 🔍 Approach
1. **SPC** — Used I-MR and X-bar/R charts to detect special cause variation.
2. **Process Capability** — Calculated Cp & Cpk.
3. **DOE** — Performed full factorial design on Temperature, Pressure, and Cycle Time.
4. **Statistical Testing** — Used ANOVA to confirm significant factors.
5. **Optimization** — Found best settings to increase average yield.

### 📊 Key Findings
- Temperature and Pressure were most impactful on yield.
- Optimized settings improved simulated yield by **~4.8%**.
- Cycle Time had strong interaction with Temperature.

### 📁 Outputs
- SPC charts
- DOE main effects & interaction plots
- ANOVA results

---

## 📂 Project 2 — FMEA & Reliability Analysis

### 📌 Objective
Rank equipment failure modes by criticality and predict time-to-failure for preventive maintenance planning.

### 🔍 Approach
1. **FMEA** — Calculated Risk Priority Number (RPN) = Severity × Occurrence × Detection.
2. **Pareto Analysis** — Identified top 20% critical failures.
3. **Reliability Modeling** — Fitted Weibull distribution to model failure times.
4. **Root Cause Analysis** — Developed fishbone diagram for top failure mode.

### 📊 Key Findings
- Motor bearing failure and temperature drift were top issues.
- Weibull β > 1.5 → Wear-out failures (preventive maintenance needed).
- Predicted **90% reliability** for ~3200 hours of operation.

### 📁 Outputs
- Pareto charts
- Weibull probability plots
- Fishbone diagram

---

## 🛠 Tools & Libraries
- **Data Analysis**: Pandas, NumPy
- **Statistics**: SciPy, Statsmodels
- **Visualization**: Matplotlib, Seaborn
- **SPC & DOE**: Control charts, full factorial design, ANOVA
- **Reliability**: Weibull analysis, Pareto, Fishbone diagrams

---

## 🚀 How to Run
```bash
# Clone the repository
git clone https://github.com/yourusername/semiconductor-projects.git
cd semiconductor-projects

# Open analysis notebooks
jupyter notebook SPC_DOE/notebooks/spc_doe_analysis.ipynb
jupyter notebook FMEA_Reliability/notebooks/fmea_analysis.ipynb
