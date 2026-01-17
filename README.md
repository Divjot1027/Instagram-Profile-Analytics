# Instagram Profile Analytics 📊

A data analysis project that scrapes (via text parsing), cleans, and visualizes Instagram profile metrics for the Bangalore tech and startup community. 

## 📝 Project Overview

This project takes raw, unstructured text data copied from Instagram profiles and converts it into a structured dataset. The goal was to analyze the "Tech Community" in Bangalore to identify key influencers, community hubs, and engagement trends.

**Key Objectives:**
* **Data Parsing:** Converting raw text blocks into structured JSON objects.
* **Data Cleaning:** Handling non-numeric values (e.g., "12.5K" to 12500) and cleaning emojis from bio text.
* **Exploratory Data Analysis:** Identifying outliers and top-performing accounts.

## 📂 Data Pipeline

1.  **Input:** Raw text chunks containing Name, Post count, Followers, Following, and Bio.
2.  **Processing:** * Split text by double newlines (`\n\n`).
    * Extracted integers from strings (e.g., removing commas, handling 'K'/'M' suffixes).
    * Stored processed data in `insta_data.json`.
3.  **Analysis:** Loaded JSON into Pandas to calculate Max/Min/Mean stats.
