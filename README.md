# 🌟 User Journey Analysis in Python 🌟

![Python Logo](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg)

## 🚀 Overview

The **User Journey Analysis** project is a powerful tool that analyzes customer behavior and the sequence of pages they visit when interacting with a product. The goal is to uncover insights that help improve the user experience, enhance the front page flow, and identify key areas for optimization. 

🔍 This analysis focuses on:
- Identifying important pages in the user journey
- Understanding user flow patterns
- Removing redundancies and irrelevant data

---

## 🛠️ Features

- **Data Preprocessing**: Clean and transform raw user journey data.
- **Behavior Metrics**: Generate key metrics like page counts, sequences, and journey length.
- **Subscription Segmentation**: Compare user behaviors across subscription plans (e.g., monthly vs. yearly).
- **Data Export**: Export the cleaned data into CSV format for further analysis.

---

## ⚡ Functions Implemented

### 1. `remove_page_duplicates`
🔹 **Purpose**: Removes sequential duplicate pages from user journey strings.

### 2. `group_by`
🔹 **Purpose**: Groups sessions of a user into a single consolidated journey string, based on the number of sessions and order.

### 3. `remove_pages`
🔹 **Purpose**: Removes unnecessary pages (like "log in") from the user journey.

### 4. Metrics Generation
🔹 Generate various metrics such as **page count**, **page presence**, **journey length**, and **destination patterns**.

---

## 📊 Data Analysis

Once the data is preprocessed, we perform several key analyses to gain actionable insights:

### Key Metrics:
- **Page Count**: How often each page appears in all user journeys.
- **Page Presence**: How often each page appears in a user’s journey (unique counts).
- **Page Destination**: What page is commonly visited after another.
- **Page Sequences**: Identifying the most frequent sequence of pages.
- **Journey Length**: Average length of a user journey in terms of page visits.
- **Subscription Segmentation**: Comparing user journeys by subscription plans.

---

## ⚙️ Installation

### Prerequisites
- Python 3.x
- `pip` for installing dependencies

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/SoufianeAzerdaoui/user-journey-analysis.git
