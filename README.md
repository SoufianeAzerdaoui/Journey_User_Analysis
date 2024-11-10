# User Journey Analysis in Python

## Project Overview

The **User Journey Analysis in Python** project aims to analyze the user behavior and page sequences of customers who bought a product. The objective is to improve the user experience by identifying key pages, common pathways, and areas of friction in the user journey. This analysis helps in enhancing the front page flow and uncovering important pages in the user experience.

---

## Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Preprocessing the Data](#preprocessing-the-data)
- [Data Analysis](#data-analysis)
- [Functions Implemented](#functions-implemented)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Project Description

This project involves preprocessing user journey data and then performing analysis to generate valuable insights. The data contains user journey sequences, and the goal is to clean, group, and analyze this data to extract patterns that can guide improvements in the user flow.

---

## Features

- **Data Preprocessing**: Cleans and transforms raw user journey data into a more analysis-ready format.
- **Metrics Generation**: Computes various metrics like page counts, page sequences, and journey length to understand user behavior.
- **Segmentation by Subscription Plans**: Analyzes data by user subscription plans (monthly, yearly) to identify behavioral differences.
- **Data Export**: Generates CSV files with cleaned and grouped data for further analysis.

---

## Preprocessing the Data

In this section, the goal is to clean and prepare the user journey data by removing duplicates, grouping sessions, and eliminating unnecessary pages. The following functions are implemented to perform these tasks:

### 1. `remove_page_duplicates`
- **Purpose**: Removes sequential duplicate pages from the user journey strings.
- **Input**:
  - `data`: The dataframe containing the raw data.
  - `target_column`: The column containing user journey strings (default is `'user_journey'`).
- **Output**: A new dataframe with cleaned-up journey strings.

### 2. `group_by`
- **Purpose**: Groups multiple sessions of the same user into a single journey string.
- **Input**:
  - `data`: The dataframe containing the raw data.
  - `group_column`: The column to group by (default is `'user_id'`).
  - `target_column`: The column containing user journey strings (default is `'user_journey'`).
  - `sessions`: The number of sessions to group (default is `'All'`).
  - `count_from`: Specifies whether to group from the first or last sessions (default is `'last'`).
- **Output**: A new dataframe containing grouped user journeys.

### 3. `remove_pages`
- **Purpose**: Removes unnecessary pages from the user journey.
- **Input**:
  - `data`: The dataframe containing the raw data.
  - `pages`: A list of pages to be removed.
  - `target_column`: The column containing user journey strings (default is `'user_journey'`).
- **Output**: A new dataframe with the specified pages removed.

---

## Data Analysis

Once the data has been preprocessed, the next step is analyzing it to extract valuable insights. The following metrics are generated during the analysis:

### 1. **Page Count**
- Counts how many times each page appears in all user journeys.

### 2. **Page Presence**
- Counts how many unique times each page appears in a user journey.

### 3. **Page Destination**
- Analyzes the most frequent follow-up pages after every page in the user journey.

### 4. **Page Sequences**
- Identifies the most frequent sequences of pages (e.g., most common 3-page sequence).

### 5. **Journey Length**
- Calculates the average length of a user journey in terms of pages.

### 6. **Subscription Plan Segmentation**
- Compares the behavior of users with different subscription plans (e.g., monthly vs annual).

---

## Functions Implemented

The following Python functions have been implemented to preprocess and analyze the user journey data:

- `remove_page_duplicates`
- `group_by`
- `remove_pages`
- Metrics generation functions like `page_count`, `page_presence`, etc.

---

## Installation

### Prerequisites

- Python 3.x
- `pip` for installing dependencies

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/SoufianeAzerdaoui/user-journey-analysis.git
