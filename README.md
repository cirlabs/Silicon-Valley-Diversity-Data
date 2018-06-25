# Silicon Valley diversity data

**NEW June 2018:**
The spreadsheet `Distributions_data_2016.csv` contains workforce distributions by job category and race for 177 of the largest tech companies headquartered in Silicon Valley.

Each figure in the dataset represents the percentage of each job category that is made up of employees with a given race/gender combination, and are based on each company's EEO-1 report.

This dataset was created through a unique collaboration with the [Center for Employment Equity](https://www.umass.edu/eeodatanet/about-us) and [Reveal](https://www.revealnews.org/?p=47103). The equity center provided Reveal with anonymized data for 177 large companies, and Reveal identified companies that have publicly released their data in this anonymized dataset. The equity center and Reveal analyzed the data independently. 

For more information on the data, read our post [here.](https://www.revealnews.org/blog/how-we-created-a-baseline-for-silicon-valleys-diversity-problem)

The spreadsheet `Reveal_EEO1_for_2016.csv` has been updated to include EEO-1s from companies PayPal, NetApp and Sanmina for 2016. The race and job categories have been modified to ensure consistency across all the datasets.


**NEW April 2018:** The spreadsheet `Tech_sector_diversity_demographics_2016.csv` contains aggregated diversity data for 177 large Silicon Valley tech companies. We calculated averages for the largest race and gender groups across job categories. For information on the aggregated data, read our post [here.](https://www.revealnews.org/blog/the-sound-of-disparity-data-directed-silicon-valley-diversity-choir/)

This repository also contains EEO-1 reports filed by Silicon Valley tech companies. Please [read our complete methodology](https://www.revealnews.org/article/how-we-analyzed-silicon-valley-tech-companies-diversity-data) for details on this data.

The data was compiled by Reveal from The Center for Investigative Reporting.

### Copyright and license

This repository and the included data are licensed under the Open Database License (ODbL) by Reveal from The Center for Investigative Reporting.

You are free to copy, distribute, transmit and adapt the spreadsheet, so long as you:

- Do not change the data in any way that introduces errors
- Credit Reveal as specified below, including linking back to Reveal as specified below.
- Inform Reveal that you are using the data in your work by emailing Sinduja Rangarajan at srangarajan@revealnews.org.
- Share the spreadsheets under the same license.

If you alter or build upon our data, you may distribute the result only under the same license. The [full legal code](https://opendatacommons.org/licenses/odbl/1.0/) explains your rights and responsibilities.

### How to credit Reveal

For the spreadsheet `Reveal_EEO1_for_2016.csv`, we require that you use the credit “Reveal from The Center for Investigative Reporting." The credit must link to https://www.revealnews.org/svdiversity unless the credit is appearing in printed media.

For the spreadsheets `Tech_sector_diversity_demographics_2016.csv` and `Distributions_data_2016.csv`, we require that you use the credit “Reveal from The Center for Investigative Reporting and The Center for Employment Equity.” The credit must link to https://www.revealnews.org/topic/silicon-valley-diversity/ unless the credit is appearing in printed media.

You must also make it clear to anyone who requests access to the data that it is available under the Open Database License. You can [link directly to the license](https://opendatacommons.org/licenses/odbl/1.0/).

## Data documentation: Distributions_data_2016.csv

### Field descriptions  
|Column name|Format|Description|
|---|---|---|
|job_category|string|Categories of jobs as classified on an EEO-1 diversity report.
|demographics|string|Racial and gender combination breakdown of the employees in each job category.|
|percentage|float| percentage of employees at a company by demographics and job category|
|company|string|companies are idenitifed by name such as Apple, Google if they've released their data publicly or to Reveal, else their classified as anonymous|

#### demographics
Race and gender combinations. Possible values are:

- Hispanic_or_Latino
- Asian
- Asian_female
- Black_or_African_American
- Black_or_African_American_female
- Female_total
- Hispanic_or_Latino
- Hispanic_or_Latino_female
- People_of_color
- Underrepresented_minorities
- Underrepresented_minorities_female
- White
- White_female
- Women_of_color

#### job_category
|Job category|Description|
|---|---|
|Executives| Executives, senior officials and senior managers|
|Managers|First- and mid-level officials and managers|
|Professionals|Includes engineers, analysts, designers, web developers, lawyers and other professionals. Does not include sales workers,  administrative  support workers and other support staff.|
|Executives and Managers|Executives and Managers combined. This cannot be calculated by adding up Executives and Manager percentages individually.|
|Executives-Professionals-Managers|Executives, Managers and Professionals combined. This cannot be calculated by adding up Executives, Managers and Professionals percentages individually.|
|Sales workers/admin support/technicians and others|Includes sales workers, administrative  support, laborers and helpers, technicians, craft workers, operatives. Includes all job categories in the EEO-1 form except Executives, Managers and Professionals|
|All workers| All workers includes executives, managers, professionals and other groups such as sales workers, administrative  support, laborers and helpers.|

## Data documentation: Tech_sector_diversity_demographics_2016.csv

### Field descriptions

|Column name|Format|Description|
|---|---|---|
|job_category|string|Categories of jobs as classified on an EEO-1 diversity report.
|race_ethnicity|string|Racial and ethnic breakdown of the employees in each job category.|
|count|integer|Aggregated employee counts broken down by race/gender and job category. |
|percentage|float|Calculated for each race/gender group within every job category. For example, percent of black executives = count of black executives/count of all executives.|

#### job_category

Companies may interpret these categories somewhat differently when reporting their numbers to the government. But generally, the job categories represent:

|Job category|Description|
|---|---|
|Executives|Executives, senior officials and senior managers.|
|Managers|First- and mid-level officials and managers.|
|Professionals|Includes engineers, analysts, designers, web developers, lawyers and other professionals. Does not include sales workers,  administrative  support workers and other support staff.|
|All workers|Total employees for the 177 companies. All workers includes executives, managers, professionals and other groups such as sales workers, administrative  support, laborers and helpers.|

For more detail about these job categories, refer to the U.S. Equal Employment Opportunity Commission’s  job classification guide [here.](https://www.eeoc.gov/employers/eeo1survey/jobclassguide.cfm)

#### race_ethnicity
Racial and ethnicity breakdown of the employees in each job category. NOTE: Adding together the counts for individual races will not equal the count in the “Totals” fields. This is because this spreadsheet does not include individual breakdowns for workers who were categorized as American Indian, Alaskan Native, Native Hawaiian, Pacific Islander or two or more races. These races make up a very small percentage of both the U.S. population and Silicon Valley workers, which makes it difficult to draw conclusions about their individual representation.

 - White
 - Asian
 - Black or African American (**Update**: modified to Black_or_African_American to be consistent across all datasets in this repository)
 - Hispanic or Latino (**Update**: modified to Hispanic_or_Latino to be consistent across all datasets in this repository)
 - All = all races including white, Asian, black or African American, and Hispanic or Latino. Also includes two or more races, Native Hawaiian or Pacific Islander, and American Indian or Alaskan Native.
 - Totals = all the totals within that job category for all races and genders

#### gender
Gender breakdown of the employees in each job category. NOTE: EEO-1 classifies all employees into either male or female, providing no options for nonbinary gender nonconforming individuals. EEO-1s do not have any information on sexual orientation. Gender totals add up to 100 percent.

- Male
- Female
- Both = both the genders in that job category

## Data documentation: Reveal_EEO1_for_2016.csv
### Field descriptions

|Column name|Format|Description|
|---|---|---|
|company|String|Company name|
|year|Integer|For now, 2016 only|
|race|String|Possible values: "American_Indian_Alaskan_Native", "Asian", "Black_or_African_American", "Latino", "Native_Hawaiian_or_Pacific_Islander", "Two_or_more_races", "White", "Overall_totals"|
|gender|String|Possible values: "male", "female". Non-binary gender is not counted in EEO-1 reports.|
|job_category|String|Possible values: "Administrative support", "Craft workers", "Executive/Senior officials & Mgrs", "First/Mid officials & Mgrs", "laborers and helpers", "operatives", "Professionals", "Sales workers", "Service workers", "Technicians", "Previous_totals", "Totals"|
|count|String|Mostly integer values, but contains "na" for a no-data variable.|

#### Update for Reveal_EEO1_for_2016.csv, June 2018:

Within the race column, value "Latino" has been changed to "Hispanic_or_Latino" to be consistent with all other datasets in this repository

Within job_category column, value "First/Mid officials & Mgrs" has been modified to "Managers" and value "Executive/Senior officials & Mgrs" has been modified to "Executives." The modifications have been made to be consistent across all the datasets in this repository.
