# Silicon Valley diversity data
This database contains EEO-1 reports filed by Silicon Valley tech companies. It was compiled by Reveal from The Center for Investigative Reporting.

Please [read our complete methodology](https://www.revealnews.org/article/how-we-analyzed-silicon-valley-tech-companies-diversity-data) for details on this data.

### Copyright and license
The EEO-1 database is licensed under the Open Database License (ODbL) by Reveal from The Center for Investigative Reporting.

You are free to copy, distribute, transmit and adapt the spreadsheet, so long as you:

- credit Reveal as specified below;
- inform Reveal that you are using the data in your work by emailing Sinduja Rangarajan at srangarajan@revealnews.org; and 
- offer any new work under the same license.

The [full legal code](https://opendatacommons.org/licenses/odbl/1.0/) explains your rights and responsibilities.

### How to credit Reveal

We require that you use the credit “Reveal from The Center for Investigative Reporting”. If it is distributed online, the credit must link to https://www.revealnews.org/svdiversity.

You must also make it clear to anyone who requests access to the data that it is available under the Open Database License. You can [link directly to the license](https://opendatacommons.org/licenses/odbl/1.0/). 

### Fields in the data

|Column name|Format|Description|
|---|---|---|
|company|String|Company name|
|year|Integer|For now, 2016 only|
|race|String|Possible values: "American_Indian_Alaskan_Native", "Asian", "Black_or_African_American", "Latino", "Native_Hawaiian_or_Pacific_Islander", "Two_or_more_races", "White", "Overall_totals"|
|gender|String|Possible values: "male", "female". Non-binary gender is not counted in EEO-1 reports.|
|job_category|String|Possible values: "Administrative support", "Craft workers", "Executive/Senior officials & Mgrs", "First/Mid officials & Mgrs", "laborers and helpers", "operatives", "Professionals", "Sales workers", "Service workers", "Technicians", "Previous_totals", "Totals"|
|count|String|Mostly integer values, but contains "na" for a no-data variable.|
