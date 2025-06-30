# Data Science Coding Challenge – Churn Prediction

## Overview
This project is part of a data science coding challenge focused on predicting **customer churn** for a video streaming service.


### Goal
Build a machine learning model that predicts whether a subscriber will **continue their subscription for another month** or **cancel**.


### Context
Subscription cancellation (“churn”) can happen for several reasons, including:

- The customer has watched all the content they wanted.
- They are too busy to use the service.
- They prefer a different platform.

Accurately predicting churn helps the company take proactive steps to **retain valuable customers**.

---

## Provided Data

1. **`train.csv`**
   - ~70% of all subscriptions (**243,787 records**)
   - Includes features describing each subscription and a target column `Churn` (*0 = retained, 1 = churned*)

2. **`test.csv`**
   - ~30% of all subscriptions (**104,480 records**)
   - Same features but **without the `Churn` label** (this is what we need to predict)

Additionally, a **`data_descriptions.csv`** file explains each feature.

---

## Train vs. Test Sets

In this challenge, you have access to two datasets that are **samples of past subscriptions** for a video streaming platform. These datasets contain information about:

- The customer
- Their streaming preferences
- Their subscription activity so far

**Datasets:**

- **`train.csv`:**
  - Contains ~70% of the overall sample (**243,787 subscriptions**)
  - Includes whether each subscription was continued into the next month (*the “ground truth”*)

- **`test.csv`:**
  - Contains the remaining ~30% (**104,480 subscriptions**)
  - Has the same information as `train.csv` but **without the target label**

**Your task:**
Using patterns you discover in `train.csv`, **predict whether each subscription in `test.csv` will be continued for another month.**

---

##  Dataset Description

Both `train.csv` and `test.csv` include:

- **One row per unique subscription**
- An identifier column: `CustomerID`
- A set of features describing the subscription, customer profile, and usage patterns

Additionally:

- `train.csv` includes the target column:
  - **`Churn`**: A binary label  
    *(0 = retained, 1 = churned)*

Apart from this label, the features are **identical** between the datasets and can be used to train your machine learning model.

A separate **`data_descriptions.csv`** file provides detailed explanations of each feature.  
Familiarize yourself with these descriptions to leverage them effectively in your modeling pipeline.
