# 💼 Billionaire Data Analysis (Excel Project)

### 🧹 Step 1: Data Cleaning

<img width="1534" height="293" alt="image" src="https://github.com/user-attachments/assets/29a2269e-5ae7-48c8-b459-11390d306514" />

To start, I cleaned up the dataset to make it ready for analysis:
- Removed duplicate entries.
- Cleaned up the Gender column by replacing "M" and "F" with full labels — "Male" and "Female".
- Combined the birthYear, birthMonth, and birthDay columns into one proper Birthdate column.
- Added a Current Date column just before Birthdate, so I could calculate the real age of each person using the =YEARFRAC() formula.
- Checked the gdp_country column for invalid characters by testing simple formulas (like =Q2+R2) — errors pointed to non-numeric values.
- Fixed those entries by using Find and Replace, then formatted the column to Number with 0 decimal places for consistency.

<img width="1586" height="587" alt="image" src="https://github.com/user-attachments/assets/03aaeb65-1aa0-4ea6-9285-373a0133e770" />

<img width="856" height="545" alt="image" src="https://github.com/user-attachments/assets/107b807b-8a5c-4905-ba6a-2cf4136810c0" />


### 📊 Step 2: Data Analysis

Once the data was clean, I dove into the analysis:

**🧠 Descriptive Stats**

I started with basic descriptive statistics using the Data Analysis Toolpak:
- Selected my data range and ran the summary tool.
- This gave me useful info like the average age, minimum and maximum net worth, and total count of people.

**🏆 Top 10 Richest Billionaires**

Next, I used a Pivot Table to find out who the Top 10 richest people were:
- Set personName as the row label, and finalWorth as the value.
- Used filters to only show the top 10, and sorted them from highest to lowest.

**📈 Billionaires by Age**

I was curious if age had any pattern — like, are older people more likely to be billionaires?
- I copied the first Pivot Table and cleared it out.
- Then used Age as both the row and value field, but changed the value to show a Count.
- To make it easier to read, I grouped the ages into 10-year ranges (30–40, 40–50, etc.).
- The result? Most billionaires fall within the 50–70 age range — interesting insight!


### 📊 Step 3: Data Visualization

To make everything easier to explore:
- I added Slicers for Industry, Self-Made, and Gender, so you can interact with the data.
- Made sure both Pivot Tables were connected to the slicers using Report Connections, so filtering updates both charts.
- Created a bar chart for the Top 10 billionaires, and another one for the age distribution.
