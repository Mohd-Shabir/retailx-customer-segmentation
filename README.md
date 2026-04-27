# 🛍️ RetailX Customer Segmentation

> Unsupervised machine learning pipeline to discover customer behavioural groups and automate segment prediction for new customers.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3+-orange?style=flat-square&logo=scikit-learn)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red?style=flat-square&logo=streamlit)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

---
---

## Table of Contents

- [Executive Summary](#executive-summary)
- [Business Problem](#business-problem)
- [Project Architecture](#project-architecture)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Skills & Tools](#skills--tools)
- [Key Results & Business Recommendations](#key-results--business-recommendations)
- [Dashboard Preview](#dashboard-preview)
- [Next Steps & Limitations](#next-steps--limitations)
- [How to Run](#how-to-run)

---

## Executive Summary

RetailX is a retail company with ~2,000 customers across varying income levels, purchase behaviours, and engagement patterns. This project applies **K-Means clustering** to segment customers into three distinct groups based on seven behavioural features — then trains a **Decision Tree classifier** to automatically assign new customers to a segment at scale.

The result is a reusable ML pipeline that outputs:
- Named customer segments with CLV and churn risk scores
- A batch predictor for new customer files
- An interactive Streamlit dashboard for business teams

**K=3 was selected** as the optimal number of clusters based on the Elbow method, Silhouette score, Davies-Bouldin index, and business interpretability.

---

## Business Problem

RetailX currently treats all customers the same — sending identical marketing campaigns regardless of spending behaviour, tenure, or engagement level. This leads to:

- Over-marketing to loyal customers who buy consistently without prompting
- Under-engaging new customers who need activation to make repeat purchases
- Wasted marketing budget on low-response segments

**Goal:** Discover natural customer groups from behavioural data and build a system that assigns new customers to the right segment automatically — enabling targeted, data-driven marketing strategies.

---
