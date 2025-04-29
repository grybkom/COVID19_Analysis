# COVID19 Analysis
Linear models and visualizations to explore the relationship between population and geospatial data with COVID19 cases and deaths.
---
## Background
The COVID-19 outbreak started in December of 2019 and was declared a pandemic by the World Health Organization on March 11th, 2020 (World Health Organization: WHO, 2024). As of August 2023, The World Health Organization (2023) estimated there were over 760 million cases and 6.9 million deaths recorded worldwide. The virus that causes COVID-19 is most often spread between people in close contact, and avoiding crowds and wearing mask is recommended to prevent the spread of COVID-19 (World Health Organization: WHO, 2023). Since close contact with others has been established as an important factor in the spread of COVID-19, it would be reasonable to assume areas with higher populations would be more adversely impacted by the disease. Here the relationship between population density and COVID-19 cases and deaths will be examined.

## Data & Methodology

- **Data**
  - The data used for this research can be found at the CSSEGISandData/COVID-19 repository: https://github.com/CSSEGISandData/COVID-19/commits?author=CSSEGISandData
- **Language**
  - R
  - [Tidyverse](https://www.tidyverse.org/)
  - [maps](https://www.rdocumentation.org/packages/maps/versions/3.4.2)

## Visualizations

![us_cases_map](https://github.com/user-attachments/assets/238c88ce-72e8-4f3e-9785-204fd66cc354)
![us_deaths_map](https://github.com/user-attachments/assets/6e1e4211-f84b-4b5f-9c7b-250f0ac50c45)

![co_county_cases_map](https://github.com/user-attachments/assets/354bee70-0066-442b-872f-3cd713224c48)
![co_county_deaths_map](https://github.com/user-attachments/assets/52920a16-6186-4f9d-9ea0-6f5ed21349d5)
![co_county_pop_map](https://github.com/user-attachments/assets/8e860beb-70ab-486b-9101-b86148e136d5)

## Results

Population was not found to be a significant factor in cases or deaths in the United States or worldwide.Linear models that included only population as the predictor resulted in p-values for population well above any acceptable significance factor. The only linear model that performed reasonably well had deaths per thousand as the response variable and included the predictors for geospatial data in the United States. In this model the predictor for latitude had a significant negative relationship with deaths per thousand. Meaning as there is a relationship between decreasing latitude, in the United States that translates to moving more southernly, and an increase in deaths related to COVID-19. 

## References
World Health Organization: WHO. (2024, February 20). Coronavirus disease (COVID-19) pandemic. https://www.who.int/europe/emergencies/situations/covid-19

World Health Organization: WHO. (2023, August 9). Coronavirus disease (COVID-19). https://www.who.int/news-room/fact-sheets/detail/coronavirus-disease-(covid-19)
