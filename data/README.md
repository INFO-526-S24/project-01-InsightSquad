# Data
-   **[Dataset]**: The National Database of Childcare Prices (NDCP) is the most comprehensive federal source of childcare prices at the county level. The database offers childcare price data by childcare provider type, age of children, and county characteristics. Data are available from 2008 to 2018. It provide estimates of childcare prices at the county level by children’s age groups and care setting (home-based or center-based providers).  

# Codebook for childcare costs Dataset
``` {r}
childcare_costs <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2023/2023-05-09/childcare_costs.csv')
counties <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2023/2023-05-09/counties.csv')
```
## Variable Names and Descriptions:

### 1. childcare_costs.csv
-   All the variables has double datatype 


| Variable    | Description |
| -------- | ------- |
| unr_16 | Unemployment rate of the population aged 16 years old or older. |
| funr_16 | Unemployment rate of the female population aged 16 years old or older. |
|munr_16 | Unemployment rate of the male population aged 16 years old or older. |
| pr_f | Poverty rate for families. |
| pr_p | Poverty rate for individuals. |
|mc_infant | Aggregated weekly, full-time median price charged for Center-based Care for infants (i.e. aged 0 through 23 months). |
| mc_toddler | Aggregated weekly, full-time median price charged for Center-based Care for toddlers (i.e. aged 24 through 35 months). |
| mc_preschool | Aggregated weekly, full-time median price charged for Center-based Care for preschoolers (i.e. aged 36 through 54 months). |
| mfcc_infant | Aggregated weekly, full-time median price charged for Family Childcare for infants (i.e. aged 0 through 23 months). |
| mfcc_toddler | Aggregated weekly, full-time median price charged for Family Childcare for toddlers (i.e. aged 24 through 35 months). |
| mfcc_preschool | Aggregated weekly, full-time median price charged for Family Childcare for preschoolers (i.e. aged 36 through 54 months). |


### 2. counties.csv
| variable  |  class  | Description |
| -------- | ------- | --------|
| county_fips_code | double | Four- or five-digit number that uniquely identifies the county in a state. The first two digits (for five-digit numbers) or 1 digit (for four-digit numbers) refer to the FIPS code of the state to which the county belongs. |
| county_name | character | The full name of the county. |
| state_name | character | The full name of the state in which the county is found. |
| state_abbreviation | character | The two-letter state abbreviation. |

		
		
		
		
		