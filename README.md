# Google Data Analytics Capstone: Cyclistic Bike-Share Case Study

This repository contains my capstone project for the **Google Data Analytics Certificate**.  
The objective of the capstone is to analyze how Cyclistic riders use bike-share bikes differently — focusing on casual riders vs annual members — in order to support potential marketing strategy decisions.

This repo includes:
- the Jupyter notebook used to clean, prepare, and analyze the data
- the official case study PDF description from Google (for reference)

---

## Business Question

> **How do annual members and casual riders use Cyclistic bikes differently?**

This comes directly from the official Google Case Study instructions.  
📄 Source: Google Case Study PDF (Cyclistic) 

---

## Repository Structure

```
.
├── cyclist-capstone-project.ipynb    # analysis notebook
├── Google_Data_Analytics_Capstone Project.pdf
└── README.md
```

> NOTE: Raw Cyclistic ride data files are NOT included in this repository due to size.  
> You will need to download the previous 12 months of ride data to run the notebook.

---

## Dataset Source (Required to Run Notebook)

Download the last 12 months of Cyclistic ride data here:  
https://divvy-tripdata.s3.amazonaws.com/index.html

These are public data files made available by Motivate International Inc.

---

## How to Run the Notebook Locally

1. Clone this repository
2. Download the trip CSV files (12 months) from the link above
3. Place all CSVs in a folder on your computer, e.g.:

```
/Users/yourname/Documents/cyclistic/raw/
```

4. Open the notebook:
```
cyclist-capstone-project.ipynb
```

5. Update the file path at the top of the notebook to match your system:

```python
data_path = "/Users/yourname/Documents/cyclistic/raw/"
```

6. Run all cells (Jupyter / VS Code / Colab)

---

## Analysis Methods Applied

- loaded and combined 12 months of CSV trip data into a single dataframe
- converted timestamps → engineered `ride_length` + `day_of_week`
- removed incomplete rows + ensured correct datetime formatting
- grouped + aggregated by rider type (member vs casual) for comparison
- produced summary tables + exploratory visualizations

---

## Notebook Output / What This Generates

- cleaned dataset with ride duration + weekly features appended
- summary statistics grouped by rider type
- visuals comparing riding patterns between user groups

---

## Possible Future Work

- add station-level location data to enable geographic mapping
- analyze seasonal differences (month or quarter)
- build a simple classification model predicting membership likelihood

---

## Tools Used

- Python (Pandas / NumPy)
- Jupyter Notebook

---
## License / Privacy Note

This capstone does **not** include any personally identifiable information.  
Cyclistic is a fictional brand created by Google for learning purposes.  
Raw data is hosted by Motivate International Inc. under a public license.
 
Raw data is hosted by Motivate International Inc. under a public license.
