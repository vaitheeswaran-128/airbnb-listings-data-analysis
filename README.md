# Airbnb Listings Data Analysis

## Project Overview
This project analyzes Airbnb listing data to understand the factors influencing **pricing, room preferences, accommodation capacity, and guest review ratings**.

The dataset contains **60,209 Airbnb listings** including room types, accommodation details, booking policies, pricing, and guest review scores. The objective of this analysis is to perform **data preparation, exploratory data analysis (EDA), and visualization** to identify important patterns that influence booking decisions and listing performance.

---

## Dataset Description

The dataset includes several features related to Airbnb listings:

### Room Information
- Room Type
- Accommodates
- Bathrooms
- Bedrooms
- Beds

### Booking & Policy Information
- Cancellation Policy
- Instant Bookable
- Cleaning Fee

### Pricing Information
- Log Price (log-transformed price variable)

### Review Metrics
- Review Scores Rating

The dataset contains **60,209 records**, with some missing values mainly in review scores and property attributes.

---

## Data Preparation

The following preprocessing steps were performed:

- Checked dataset structure and column information
- Identified missing values
- Handled missing values using:
  - **Median imputation** for bathrooms, bedrooms, and beds
  - **Mode imputation** for categorical variables
- Checked for duplicate records
- Verified data types

Approximately **22.6% of values were missing in the review score column**, which required careful handling.

---

## Exploratory Data Analysis (EDA)

### Univariate Analysis

The distribution of the **accommodates** variable shows that most listings accommodate **1–4 guests**, indicating that Airbnb properties mainly target small groups and couples.

Visualization used:
- Histogram

---

### Room Type Distribution

Analysis of room types shows:

- **Entire home/apartment** is the most preferred listing type
- **Private rooms** are the second most popular
- **Shared rooms** have significantly lower demand

This suggests travelers prefer privacy and full property rentals.

---

### Cancellation Policy Analysis

The distribution of cancellation policies shows:

- **Strict policy** – 43.8%
- **Flexible policy** – 30.4%
- **Moderate policy** – 25.7%

Hosts tend to prefer stricter cancellation policies to reduce last-minute cancellations.

---

### Accommodation Capacity Analysis

Room types serve different guest segments:

- **Entire homes/apartments** support larger groups
- **Private rooms** typically accommodate **2 guests**
- **Shared rooms** mainly accommodate **1–2 guests**

This indicates that entire homes are more versatile for different group sizes.

---

### Review Score Analysis

Guest satisfaction across room types shows:

- Median ratings are **close to 100** across all room types
- **Entire homes** have stable and consistent ratings
- **Private rooms** show slightly more variation
- **Shared rooms** show the highest variability in ratings

This indicates shared rooms may provide inconsistent guest experiences.

---

## Visualizations Used

The following visualizations were used in the analysis:

- Histogram – Distribution of accommodation capacity
- Count Plot – Room type distribution
- Pie Chart – Cancellation policy distribution
- Bar Plot – Total accommodates per room type
- KDE Plot – Accommodation distribution by room type
- Violin Plot – Review score distribution by room type

These visualizations help identify patterns in guest preferences and listing performance.

---

## Key Insights

Important findings from the analysis include:

- Entire homes/apartments dominate Airbnb listings
- Private rooms are commonly designed for couples or small groups
- Shared rooms are the least popular option
- Review scores are generally very high across all listings
- Property size (beds and bedrooms) has stronger influence on pricing compared to bathrooms
- Guest experience factors such as cleanliness, service, and location may influence reviews more than property size

---

## Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure
