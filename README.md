# Poland Apartment Prices: Listings vs Transactions

Analysis of apartment prices in 13 Polish cities. The project compares asking prices from online listings with real transaction prices published by the National Bank of Poland (NBP).

## Data
- **Kaggle: Apartment Prices in Poland** (author: krzysztofjamroz). Monthly listings, Aug 2023 - Jun 2024. https://www.kaggle.com/datasets/krzysztofjamroz/apartment-prices-in-poland
- **NBP: housing price database (BaRN)**. Quarterly offer and transaction prices per m², 17 cities, up to Q2 2026. Source: nbp.pl

Raw data files are not included in this repository.

## What I did
- Combined 11 monthly files into one table (195,568 rows) and removed repeated listings, leaving 92,967 unique listings
- Calculated price per m² and compared cities
- Studied Warsaw: price by distance from the centre, rooms and amenities
- Compared sale prices with rent to estimate gross rental yield
- Cleaned the NBP Excel file and joined it with the Kaggle data
- Compared listing prices with NBP transaction prices for Q2 2024

## Key findings
- Asking prices are higher than transaction prices in all 13 compared cities (gap from 1.9% to 12.3%, median 8.6%).
- The gap is largest in Białystok and smallest in Szczecin.
- Warsaw is the most expensive market: about 16,300 PLN/m² in transactions in Q2 2024, about 16,700 PLN/m² in Q2 2026 (NBP).

## Limitations
Kaggle data shows listing prices (median), while NBP shows mean prices, so the numbers are close but not identical. Kaggle data ends in June 2024.

## Tools
Python, pandas, matplotlib, Google Colab

## Author
Zoriana Kutsa
