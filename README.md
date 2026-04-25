# 🕵️‍♂️ LAPD Crime Data Analysis & Strategic Insights

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3.0+-blue.svg)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4+-orange.svg)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11+-green.svg)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-yellow.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Project Idea](#project-idea)
- [Key Objectives](#key-objectives)
- [Tools & Technologies](#tools--technologies)
- [Dataset Description](#dataset-description)
- [Project Workflow](#project-workflow)
- [Project Timeline](#project-timeline)
- [Project Insights](#project-insights)
- [KPIs](#kpis)
- [Instructor](#instructor)
- [Future Improvements](#future-improvements)
- [Installation](#installation)
- [Project Files](#project-files)
- [Contact](#contact)

---

## 📖 Project Overview

Urban safety and crime prevention rely heavily on data-driven decision-making. This project analyzes a comprehensive dataset from the **Los Angeles Police Department (LAPD)** to explore crime distribution, frequency patterns, and victim demographics across the city.

Using Python-based EDA techniques, this project uncovers the "when," "where," and "who" of criminal activities in Los Angeles, providing a foundation for predictive policing and public awareness.

---

## 💡 Project Idea

The project transforms a raw LAPD dataset (185,000+ records) into a "Golden Record" through rigorous cleaning and feature engineering. By resolving missing values in weapon descriptions and correcting logical inconsistencies in victim ages, we perform a deep exploratory analysis to identify significant social and temporal trends in urban crime.

---

## 🎯 Key Objectives

- 🔄 **Data Engineering**: Clean and preprocess raw crime data (handling 112k+ nulls, formatting dates).
- 🕒 **Temporal Analysis**: Identify peak crime hours and distribution across days of the week.
- 🌍 **Geospatial Hotspots**: Rank the most active patrol divisions (e.g., Central, Hollywood).
- 👥 **Demographic Profiling**: Analyze crime impacts based on victim age, sex, and descent.
- 🛠️ **Visual Storytelling**: Build an intuitive dashboard of findings using Seaborn and Matplotlib.

---

## 🛠️ Tools & Technologies

| Category | Technologies |
|----------|-------------|
| **Programming** | Python |
| **Data Processing** | pandas, numpy |
| **Visualization** | Matplotlib, Seaborn |
| **Development** | VS Code, Jupyter Notebook |

---

## 📊 Dataset Description

The dataset (`crimes.csv`) contains **185,000+ records** including:
- `DR_NO`: Division of Records Number (Unique ID)
- `DATE OCC`: Date the crime occurred
- `TIME OCC`: Military time of occurrence
- `AREA NAME`: Geographic patrol division (e.g., Hollywood, Central)
- `Crm Cd Desc`: Description of the crime type
- `Vict Age`: Age of the victim
- `Vict Sex` & `Vict Descent`: Demographic identifiers
- `Weapon Desc`: Description of weapon used

---

## 🔄 Project Workflow

### 1. 🧹 Data Cleaning & Preprocessing
- Converted `Date Rptd` and `DATE OCC` to standard datetime objects.
- Extracted `hour` feature from the text-based `TIME OCC` column.
- Handled massive missing data in `Weapon Desc` by filling with "Unknown".
- Corrected invalid `Vict Age` records (0 or negative) using **Median Imputation**.
- Mapped descent codes (H, W, B, etc.) to full descriptive titles for clarity.

---

### 2. 📈 Exploratory Data Analysis (EDA)
- **Time Distribution**: Analyzed which hours see the highest crime spikes.
- **Location Profiling**: Identified areas with the highest report density.
- **Demographic Analysis**: Examined victim characteristics and targeted groups.
- **Weaponry Trends**: Evaluated the frequency of weapon-related incidents.

---

### 3. 📊 Data Visualization
- **Line Graphs**: Tracking 24-hour crime trends.
- **Horizontal Bar Charts**: Ranking top 10 crime areas and victim descents.
- **Heatmaps**: Correlating crime frequency with days and hours.
- **Pie Charts**: Distribution of victim gender and crime types.

---

## 💡 Project Insights

- 🕒 The Midday Peak: Analysis confirms 12:00 PM as the peak hour for reporting, often linked to default logging for identity theft.

- 📍 Danger Zones: The Central and Hollywood areas report the highest volumes of criminal activity.

- 🎭 Demographics: Victims of Hispanic/Latin/Mexican descent show the highest frequency in records, followed by White and Black communities.

- 👦 Age Trends: After correcting invalid entries, the median victim age sits in the late 30s, indicating a specific targeted demographic.

## 📊 KPIs (Key Performance Indicators)

- ✅ Data Quality: 100% resolution of invalid ages and standardized datetime formats.

- ✅ Code Reproducibility: Clean, documented Python scripts within VS Code environment.

- ✅ Analytical Depth: Comprehensive coverage of time, location, and demographic metrics.

- ✅ Documentation: High-quality README and structural organization.

## 🧑‍🏫 Instructor
**Under the supervision of**: **Dr. Dina Ezzat**

## 🚀 Future Improvements
- [ ] Integrate Geographic Information System (GIS) tools for interactive mapping.

- [ ] Implement Machine Learning models to predict high-crime periods.

- [ ] Perform sentiment analysis on crime descriptions.
