
# EDA Google Play Store

This document summarizes the steps taken during the Exploratory Data Analysis (EDA) of the Google Play Store dataset. It covers data loading and basic exploration.

### 1. Import Required Libraries

These are the core Python libraries used for data analysis and visualization.

import pandas as pd \
import numpy as np \
import matplotlib.pyplot as plt \
import seaborn as sns

### Load the Dataset

Read the dataset and check its dimensions.

df = pd.read_csv("googleplaystore.csv") \
df.shape\
df.head()

### 3. Basic Exploration

Get a quick overview of the dataset.

df.info() \
df.describe(include='all') \
df.columns

### Missing Values Analysis

After loading the dataset, a full check for null values was performed to understand data quality:

### Convert Columns to Numeric

Some columns are stored as text and must be cleaned before converting.

### Visualizing Missing Values

To clearly understand where the dataset has gaps, a heatmap bar plot was used.
This plot highlights missing values column-wise so you can instantly see which features need cleaning.