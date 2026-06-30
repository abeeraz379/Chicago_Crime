# Chicago Crime (Time Series Analysis & Forecasting Project)
### Data Source/ Chicago Data Portal: Crimes 2001 to Present
- Data Description: All Crimes that were reported in the city of Chicago and their details View Preview
- Includes: type of crime, exact date/time, lat/long, district/ward, whether there was an arrest, etc.
---
# Used Libraries
### pandas / numpy /matplotlib.pyplot / os / zipfile / glob / holidays /seasonal_decompose
---
# Stakeholder Questions

## Topic 1) Comparing Police Districts
- Which district had the most crimes in 2022?
  - sol / Most crimes (2022): District 8
- Which had the least?
  - sol /Least crimes (2022): District 31

## Topic 2) Crimes Across the Years:
- Is the total number of crimes increasing or decreasing across the years?
  - sol/ Overall trend: Crime is decreasing from 2001 → 2022
- Are there any individual crimes that are doing the opposite (e.g., decreasing when overall crime is increasing or vice-versa)?
  - sol/ Some crimes increase instead of decrease:
-- Motor Vehicle Theft
-- Weapons Violation
-- Criminal Sexual Assault
-- Stalking
-- Human Trafficking
  <img width="876" height="547" alt="تنزيل (1)" src="https://github.com/user-attachments/assets/21723caf-8799-497a-aa65-235e4e6d6eef" />
  <img width="1031" height="547" alt="تنزيل" src="https://github.com/user-attachments/assets/a596f237-f1cd-4bd5-8486-d7c245446486" />


## Topic 3) Comparing AM vs. PM Rush Hour:
- Are crimes more common during AM rush hour or PM rush hour?
You can consider any crime that occurred between 7 AM - 10 AM as AM rush hour
You can consider any crime that occurred between 4 - 7 PM as PM rush hour.
  - sol / PM rush hour has more crime
- Answer the question: What are the top 5 most common crimes during AM rush hour? What are the top 5 most common crimes during PM rush hour?
  - sol /Theft - Battery - Criminal Damage -Assault - Burglary
- Answer the question: Are Motor Vehicle Thefts more common during AM rush hour or PM Rush Hour?
  - sol / More common in PM

## Topic 4) Comparing Months:
- Answer the question: What months have the most crime? What months have the least?
  - sol / Highest: Summer (June–August) - Lowest: Winter (Jan–Feb)
- Answer the question: Are there any individual crimes that do not follow this pattern? If so, which crimes?
  - sol /Some crimes do NOT follow this pattern: Burglary - Motor Vehicle Theft
  <img width="876" height="556" alt="تنزيل (2)" src="https://github.com/user-attachments/assets/f33134d3-b38b-4d92-9050-446242e8672f" />
  <img width="1032" height="547" alt="تنزيل (3)" src="https://github.com/user-attachments/assets/f1e5a0b5-33d8-4e65-9d20-9618f04a5eb4" />

## Topic 5) Comparing Holidays:
- Answer the question: What are the top 3 holidays with the largest number of crimes?
  - sol / Independence Day-  Halloween-  New Year
- Answer the question:  For each of the top 3 holidays with the most crime, what are the top 5 most common crimes on that holiday?
  - sol /Theft - Battery - Assault -Criminal Damage

## Topic 6) What cycles (seasonality) can you find in this data?
- Make sure to select the data of interest and resample it to the frequency you want. (For suggestions, See the "Suggested data to check for seasons" list at the bottom of this topic.)
Use statsmodels.tsa.seasonal.seasonal_decompose() to decompose the time series.
- Note: seasonal_decompose cannot read data resampled as minutes or smaller, and if you try seconds, you will crash your computer. Keep your resampling at hours or more.

- Show and describe each cycle you can find.
(Hint: If your seasonal results are too dense to read, try zooming in to look at just one year or one month and try different levels of resampling).
- Answer the question: How long is a cycle?
  - sol / 12 months
- Answer the question: What is the magnitude of the cycle? (Compare min and max).
  - sol /Max seasonal ≈ high summer - Min seasonal ≈ winter

<img width="1105" height="753" alt="تنزيل (4)" src="https://github.com/user-attachments/assets/52a30bb9-a768-4038-abab-5334be6e274c" />
<img width="630" height="470" alt="تنزيل (5)" src="https://github.com/user-attachments/assets/fc417562-e318-4b53-894e-50223775a8bd" />

---
## Solution Code : https://github.com/abeeraz379/Chicago_Crime/blob/main/Chicago_Crime_Data.ipynb

