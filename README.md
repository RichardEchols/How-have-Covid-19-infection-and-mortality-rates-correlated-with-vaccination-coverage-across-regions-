**How have Covid-19 infection and mortality rates correlated with vaccination coverage across regions over the pandemic timeline?**





![T-cell-1](https://github.com/RichardEchols/How-have-Covid-19-infection-and-mortality-rates-correlated-with-vaccination-coverage-across-regions-/assets/125469793/a5d9223d-ff6d-4f1b-9297-04f9b65389e2)





**Background:**


In the wake of the global crisis brought on by COVID-19, data analysis has become a key tool in understanding the impact of the pandemic. While the world grappled with the virus, data analysts like myself have turned to the numbers for insights. This project is born out of a need to comprehend the scale and severity of COVID-19 across different regions and how it correlates with variables such as population density and vaccination rates. My journey through this dataset is also a personal one, as it mirrors the path of the pandemic which has touched the lives of so many around me.





**Questions:**


This analysis aims to answer several pressing questions regarding the COVID-19 pandemic:

* What is the correlation between total cases and total deaths across different locations?
* How does the percentage of the population infected compare across countries?
* Which countries have the highest infection rate when adjusted for population?
* How do continents differ in terms of total deaths and death rate per population?
* What percentage of the global population has been vaccinated over time?





**Main Findings:**



Through meticulous SQL queries and data manipulation, I uncovered several key findings:

* The death percentage varied significantly across countries, which may point to differences in healthcare systems, reporting accuracy, or virus strains.
* The infection rates when adjusted for population size revealed that densely populated countries did not always have higher infection rates, suggesting the effectiveness of public health measures.
* Vaccination data showed that the rollout was uneven across different locations, with some countries achieving high vaccination numbers rapidly, while others lagged behind.






**Conclusions:**



The conclusions drawn from this analysis are as follows:

* There is a wide disparity in COVID-19 impact and response effectiveness across different regions.
* Death percentages and infection rates do not always correlate with population size, indicating a complex interplay of factors influencing pandemic outcomes.
* Vaccination progress, while promising, is uneven globally, highlighting the need for international cooperation in pandemic response.



**Original Dataset**


<img width="1241" alt="Screenshot 2023-11-14 at 2 24 09 PM" src="https://github.com/RichardEchols/How-have-Covid-19-infection-and-mortality-rates-correlated-with-vaccination-coverage-across-regions-/assets/125469793/e33ec389-68f9-47c8-9df9-370cdaff1441">







**Process:**

The journey through the data began with a careful selection of relevant datasets from the 'CovidDeaths' and 'CovidVaccinations' tables, ensuring that only records with non-null continent fields were considered to maintain the integrity of the analysis.

**Data Extraction:**

Initial queries fetched core data, including location, dates, total cases, new cases, and total deaths, all sorted to facilitate chronological analysis.

**Calculating Key Metrics:**

Computation of critical indicators such as death percentages and population infection percentages allowed for a deeper understanding of the virus's lethality and reach.


**Comparative Analysis:**

By focusing on 'states' within the dataset, I was able to draw direct comparisons between different areas, particularly looking at case and death counts in relation to population figures.


**Aggregation and Grouping:**

Aggregated data provided the highest infection counts and death counts, which were then used to rank countries and continents, revealing the areas most impacted by the pandemic.


**Temporal Analysis:**

Global numbers were summarized over time to track the pandemic’s progress and the corresponding death percentages, offering a dynamic view of the situation as it unfolded.


**Vaccination Rollout:**

Joining the CovidDeaths and CovidVaccinations datasets enabled an analysis of the vaccination efforts against the backdrop of existing population data.


**Advanced SQL Techniques:**

Utilizing Common Table Expressions (CTEs) and temporary tables, I managed to perform more complex, cumulative calculations, such as rolling counts of vaccinated individuals.

**Data Persistence:**

For future reference and visualizations, a view named 'PercentPopulationVaccinated' was created, which stored the calculated vaccination percentages over time.
