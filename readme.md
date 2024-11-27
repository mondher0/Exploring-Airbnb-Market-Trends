# Airbnb Short-Term Rental Market Analysis in New York

This repository contains a data analysis project aimed at understanding the short-term rental market in New York City using Airbnb listing data from 2019. The analysis leverages data from three key sources:

- `airbnb_price.csv`: Contains information about listing prices and locations.
- `airbnb_room_type.xlsx`: Contains information about the descriptions and room types (e.g., shared, private, entire home).
- `airbnb_last_review.tsv`: Contains details on the host names and the dates of the last reviews.

## Project Goals

The analysis aims to provide insights into the following areas:
1. **Earliest and Most Recent Reviews**: Identifying the dates of the first and last reviews from the dataset.
2. **Private Room Listings**: Counting the number of private room listings.
3. **Average Listing Price**: Calculating the average nightly price of all listings.

## Key Analysis Steps
- Load and preprocess data from CSV, TSV, and Excel formats.
- Clean and format dates to calculate the earliest and most recent review.
- Calculate the number of private room listings.
- Compute the average listing price rounded to two decimal places.
- Combine the results into a DataFrame for reporting.

## Results
The final result is a single-row DataFrame (`review_dates`) that contains:
- `first_reviewed`: Date of the earliest review.
- `last_reviewed`: Date of the most recent review.
- `nb_private_rooms`: Number of private room listings.
- `avg_price`: Average listing price (rounded to two decimal places).

## Setup

1. Clone this repository to your local machine.
2. Install the necessary dependencies using the following:
   ```bash
   pip install pandas openpyxl
