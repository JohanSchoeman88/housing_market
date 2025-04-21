  ## Davidson County redfin/school/crime data

1. Executive Summary
I want to explore the intersection between public education, housing affordability, and community safety in Nashville. Using ZIP-level data from 2012–2024, the goal is to uncover how school performance, housing prices, and crime rates interact — and how those dynamics have changed over time. The final product will be a Power BI 
dashboard that lets users explore trends and relationships across neighborhoods.

2. Motivation

Nashville is growing rapidly, and with it comes increasing tension between affordability, school quality, and safety. As families decide where to live, they're balancing home prices against the availability of good schools and safe neighborhoods. This project aims to make those trade-offs visible by unifying education, crime, and housing data into a single dashboard. The motivation stems from the desire to better understand systemic equity across ZIP codes and provide a data tool that may help the user make better informed decisions.

3. Data Question

a. How do school performance, crime, and housing prices interact across ZIP codes in Nashville from 2012 to 2024?
b. Which ZIP codes have achieved high educational outcomes despite affordability or safety concerns?
c. Correlations of trendline between school avg grades, home prices, and total crime rates.

4. Minimum Viable Product (MVP)

The final product will be a multi-page PowerBI Dashboard with:

ZIP-Level Overview: Map and bar charts showing key metrics by area
Housing & Crime: Line and bar charts exploring price and safety trends
School Performance & Crime: Visuals highlighting the relationship between education and safety
School Performance & Housing: Insights on affordability vs. school quality
Slicers by year, ZIP, subject, grade


5. Data Sources

    School Assessment Data (2012 to 2024)
Source: TN Department of Education (tn.gov)

    Crime Data
Source: Metro Nashville Police Open Data Portal (data.nashville.gov)

    Housing Data
Source: Redfin ZIP Code Tracker (web-scraped + filtered), (www.redfin.com)

    ZIP Code Reference
Source: data.gov

6. Known Issues and Challenges

School assessment data varies across years required column standardization
ZIP code mismatches between datasets due to naming inconsistencies
Large dataset size caused memory issues in Python solved by low_memory=False
Crime dataset included out-of-state records  filtered to Davidson County
Power BI forced many-to-many joins  resolved through a zip_year_key


No API keys are required for this project. All datasets are CSV-based and locally stored.

