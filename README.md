The aim of this project is to examine the relationship between national food availability and adult obesity. In many countries, the amount of food available has been increasing over the years, and at the same time, obesity levels have also risen. This project answers the question: “How does national food availability relate to adult obesity over time?”

To explore this, two major international datasets were used that provide information on food supply, population, and adult obesity for many countries across multiple years. By cleaning, merging, and analysing these datasets, a visualisation was created to help explain how food availability and obesity change together.

The first dataset is the Food Balance Sheet from the Food and Agriculture Organization (FAO). It provides information about how much food is available in each country. The main variable used from this dataset is food supply, measured in kilocalories per person per day. The second dataset is the Obesity Among Adults dataset from the World Health Organization (WHO). It reports the percentage of adults who are obese for each country and year. Both datasets include information across time, countries, and numerical values, making them suitable for comparing food availability with adult obesity and for creating a meaningful visualisation.

- Data Cleaning
1. Cleaning the FAO Food Supply Dataset:
A new numeric year column was added, and only the two required elements were selected:
Food supply (kcal/capita/day)
Total population – both sexes
Missing or inconsistent values were removed, and important columns were converted to numeric types so the data could be used in charts and calculations.
2. Cleaning the WHO Obesity Dataset:
For the WHO dataset, only the indicator “Prevalence of obesity among adults, both sexes” was selected. The numeric obesity percentage for each country and year was then extracted.

- Data Merging
1. Merging the FAO Dataset:
A left join was used, meaning all food supply values were kept even if population data was missing. This approach helped prevent the loss of important records.
2. Merging with the WHO Obesity Dataset:
The combined FAO table was merged with the WHO obesity dataset using country and year as the common keys.

- Sanity Checks:
Kilocalories per capita must be a positive number.
Obesity percentage must be between 0 and 100.
Visualisation Methodology
To understand the relationship between food availability and adult obesity, an animated bubble scatter plot was created. This visualisation displays multiple pieces of information simultaneously.

- Key Findings
 1. Positive Relationship:
Countries with higher food availability (more daily calories) usually have higher adult obesity levels. As calorie supply increases, obesity tends to rise.
 2. Stronger Relationship Over Time:
From 2010 to 2022, most countries move upward and to the right on the chart. This indicates that both food supply and obesity percentages increased over the years.
 3. Population Influence:
Population size does not change the direction of the trend, but it affects the scale of impact.
Large-population countries have a greater overall impact because even small changes in obesity affect millions of people.
Small countries may have high obesity rates, but their global impact is smaller.
