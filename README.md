# User Journey Analysis in Python

## Overview

The **User Journey Analysis** project analyzes customer behavior and page sequences to improve user experience. It processes raw data to identify key pages, common paths, and areas needing optimization for a smoother user journey.

---

## Features

- **Data Preprocessing**: Clean and transform user journey data.
- **Metrics Generation**: Calculate page counts, sequences, journey length, and more.
- **Subscription Segmentation**: Compare behavior across different subscription plans.
- **Data Export**: Generate CSVs for further analysis.

---

## Functions Implemented

- `remove_page_duplicates`: Cleans sequential duplicate pages.
- `group_by`: Groups multiple sessions into a single journey.
- `remove_pages`: Removes unnecessary pages from journeys.
- Metrics generation functions like `page_count`, `page_presence`, etc.

---

## Installation

### Prerequisites

- Python 3.x
- `pip` for installing dependencies

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/SoufianeAzerdaoui/user-journey-analysis.git
