**<h2>Overview of the Zomato Data Analysis
Analyzing restaurant data from Zomato, combining it with country details to explore trends in ratings, cuisines, and locations.</h2>**

**1. Data Loading and Inspection**
Data Files

zomato.csv (main restaurant dataset)

Country-Code.xlsx (maps country codes to country names)

Inspecting the data structure: shape (9551 rows × 21 columns)

Checking data types, missing values (Cuisines column has 9 missing entries).

**2. Missing Data Analysis**
Used .isnull() and .mean() to quantify missingness.

Plotted a heatmap of null values.

Found that Cuisines is the only column with missing values.

**3. Country Mapping**
Merged zomato.csv with Country-Code.xlsx on Country Code.

This added a Country column for each entry.

Top 3 countries by restaurant count:

India, USA, UK (pie chart created).

**4. Ratings Analysis**
Grouped by Aggregate rating, Rating color, Rating text, and counted reviews.

Created:

Bar plot of Aggregate Rating counts, color-coded by rating color.

Count plot of restaurants by Rating color.

Countries with 0 Rating (White color)
India, Brazil, USA, UK

**5. Currency by Country**
Grouped countries by the currency used.

**6. Online Delivery Analysis**
Found that only India and UAE have restaurants with Has Online delivery = Yes.

**7. Top Cities Analysis**
Listed most frequent cities:

New Delhi, Gurgaon, Noida, Faridabad, Ghaziabad

Pie chart showing top 5 cities.

**8. Cuisine Analysis**
Split the Cuisines column into individual items.

Flattened into one list and prepared for frequency analysis to identify top cuisines.

**Key Insights:**

Dataset is dominated by Indian restaurants.

India and UAE support online delivery.

Most popular cuisines likely include North Indian, Chinese, Fast Food, Continental, Italian.

A large share of restaurants have high ratings, but India also has many unrated entries.
