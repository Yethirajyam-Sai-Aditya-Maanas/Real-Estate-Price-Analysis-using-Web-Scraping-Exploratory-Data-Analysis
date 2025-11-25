# Real-Estate-Price-Analysis-using-Web-Scraping-Exploratory-Data-Analysis\
🏡 Real Estate Web Scraping & EDA (MagicBricks – Hyderabad)
A Complete Data Analyst Project Done in ONE Jupyter Notebook

This project covers the end-to-end data workflow:

✔ Web Scraping (Requests + BeautifulSoup)
✔ Data Cleaning & Feature Engineering
✔ Exploratory Data Analysis
✔ Business Insights

Everything is implemented inside a single notebook for easier review and reproducibility.

📌 1. Business Problem

Real estate buyers and investors need clear analytics on:

Price variations across localities

Relationship between area and price

Effect of BHK, furnishing, bathrooms on price

Comparison between Gachibowli & Kondapur

The goal is to build a complete analytical dataset and extract actionable insights.

📌 2. Objective of the Project

Scrape real estate property listings from MagicBricks

Clean and preprocess the dataset for EDA

Identify price drivers in Hyderabad real estate

Present meaningful business insights using visualizations

Publish the project on GitHub and add it to the resume

📌 3. Web Scraping Details
Website Used: MagicBricks
Methodology:

Sent GET requests to each paginated URL

Parsed listing cards using BeautifulSoup

Extracted structured fields (Title, Price, Area, BHK, Bathroom…)

Cleaned text using Regex

Stored data into Pandas DataFrame

Total Extracted Records: 2725

No Selenium used → lightweight, fast, stable.

📌 4. Summary of the Data

Final dataset: 2725 rows × 12 columns

Core Features
Feature	Description
Property_Type	Apartment / Villa
BHK	Bedrooms
Price_Min / Max / Avg	Clean numeric price (₹)
Area_Clean	Super built area in sqft
Furnishing	Furnished/Semi/Unfurnished
Parking	Parking availability
Bathrooms	1–6
Transaction Type	New / Resale
Locality	Gachibowli / Kondapur / Whitefields…
Description	Short text
📌 5. Data Cleaning Steps (Performed in Notebook)

Converted price formats like ₹1.49 Cr → 14900000

Cleaned area like "1200 sqft" → 1200

Removed noisy columns:

Project_Name

Status

Possession

Builder Name

Lat/Long

Price text

Removed duplicates

Cleaned text for Furnishing, Parking

Filled missing values where appropriate

Converted all numerical fields to correct dtypes

📌 6. Exploratory Data Analysis Steps
Univariate

Distribution of Price

Distribution of Area

BHK Counts

Furnishing breakdown

Parking availability

Bivariate

Price vs Area

Price vs BHK

Locality vs Price

Furnishing vs Price

Bathrooms vs Price

Multivariate

Correlation heatmap

Scatter plots for numerical relationships

📌 7. Key Business Insights
🏷️ 1. Area is the strongest driver of price

Correlation ≈ 0.83

🏷️ 2. Furnished properties cost 25–35% higher
🏷️ 3. 3 BHK units are the most commonly listed
🏷️ 4. Gachibowli is consistently more expensive than other localities
🏷️ 5. Villas are rare but priced extremely high (₹4–18 Cr)
📌 8. Conclusion

✔ Successfully scraped real Hyderabad property data
✔ Clean dataset prepared with 12 meaningful features
✔ Visual analysis explains major price factors
✔ Ready for regression modeling & dashboards
✔ Strong resume-friendly case-study

📌 9. Challenges Faced

MagicBricks provides inconsistent HTML structures

Many fields missing across listings

Price & area needed heavy Regex cleaning

Duplicate listings suppressed manually

Some listings contained long unstructured descriptions

📌 10. Tech Stack
Component	Tools
Language	Python
Scraping	BeautifulSoup, Requests
Data Cleaning	Pandas, NumPy, Regex
Visualization	Matplotlib, Seaborn
Notebook	Jupyter
📌 11. How to Run This Project
pip install -r requirements.txt
jupyter notebook


Open:

notebook/Real_Estate_WebScraping_Cleaning_EDA.ipynb
