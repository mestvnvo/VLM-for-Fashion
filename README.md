# Senior Project: Product Classification and Color Discretization Using Vision-Language Models

## Overview

This repository contains the Jupyter Notebook for my senior project, where I researched and utilized a vision-language model, **LLaVA_NeXT**, to classify product types and identify primary colors from product names and images. The project aimed to address the challenge of abstract and vague color names (e.g., "starfish," which could represent brown, orange, or red) by accurately predicting the main colors, and generalizing product types (e.g., sweaters to outerwear or joggers to bottoms).

The project relied on product data scraped for Sleeve's use, processed, and evaluated using a **Google Sheets** dataset.

## Files

### 1. [VLM4Fashion.ipynb](VLM4Fashion.ipynb)

This Jupyter Notebook implements the following:

- Utilizes **LLaVA_NeXT**, a vision-language model.
- Processes product names and images through prompting to classify product types and colors.
- Provides detailed analysis and comparison of raw data vs. predicted vs. labeled outputs.
- Metrics of model accuracy:
  - **Color Prediction Accuracy:** 66.96%
  - **Product Type Prediction Accuracy:** 74.29%

### 2. [Google Sheets Dataset](https://docs.google.com/spreadsheets/d/17WsSVU40pRwsrhHW8_Sep1oGSPQUIX67TdqsDG9de40/edit?usp=sharing)

The dataset is structured into three sheets:

- **Sheet 1:** Contains raw, scraped data, including the product's name, image URL, product type, and color.
- **Sheet 2:** Contains the labeled color/product type and the model's predictions.
  - Color prediction accuracy: 66.96%
  - Product type prediction accuracy: 74.29%
- **Sheet 3:** Merges all data—raw, labeled, and predicted.
  - Raw vs. labeled color accuracy: 22.06% 
  - Prediction vs. labeled color accuracy: 66.96%, showing a **44.9% improvement**.
  - Raw vs. labeled product type accuracy: 8.5%
  - Prediction vs. labeled product type accuracy: 74.29%, showing a **65.79% improvement**.
  - ANDing both raw attributes (color and product type) resulted in a 1.64% accuracy.
  - ANDing both predictions resulted in a 50.64% accuracy, indicating a **49.01% improvement**.

 ## Results

The model demonstrated significant improvements over raw data classification:

- **Color accuracy improved** by 44.9%.
- **Product type accuracy improved** by 65.79%.
- **Overall accuracy** for both attributes improved by 49.01%.
