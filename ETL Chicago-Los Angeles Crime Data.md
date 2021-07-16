ETL-Project

Objective and Scope:
The purpose of this project is to perform what is commonly referred to as ETL. ETL stands for Extract, Transform, and Load. This is a practice that is crucial in creating data that is clean and usable for the purpose of analyzing, storing, etc. The process can be broken down into its individual parts: extracting or acquiring the data from a source or sources, transforming or cleaning it into a form that is more readable and usable, and finally loading the data into a database or table.

Extract:
For this project, data was collected from two city websites. The first dataset that was extracted outlines crime in Chicago (https://data.cityofchicago.org/Public-Safety/Crimes-One-year-prior-to-present/x2n5-8w5q/data) in the format of a CSV file. This dataset reflects reported incidents of crime (with the exception of murders where data exists for each victim) that have occurred in the city of Chicago over the past year, minus the most recent seven days of data. This data is being extracted from the Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system.
The second dataset reflects incidents of crime in the city of Los Angeles dating back to 2020  (https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8/data in the format of a CSV file. This data is transcribed from original crime reports that are typed on paper, thus possibly providing some inaccuracies within the data.

Transform:
To transform this data into a usable form, Pandas, was utilized. Pandas proved to be highly effective due to its ability to easily load data from a file into a pandas data frame, where data can be manipulated into a form that we can find relevant to our analysis.
First, the city of Chicago and Los Angeles CSV files was read into a pandas data frame. Then removal was done on columns that were not present in the Los Angeles dataset. In addition, two text columns were combined, and the columns were renamed to be the same as the Los Angeles data. Additionally, as a precaution, any null values in our data frames were dropped.

Load:
Lastly, a pandas.concant function was used to append both datasets. This resulted in two CSV files being exported into a combined CSV dataset.

Conclusion:
The requirements for this project were completed successfully. The purpose was not to perform an analysis on the data, but rather to prepare the data in a way that an analysis would not be limited by any inconsistencies or formatting errors due to how the data is stored. 
After ETL was performed on the datasets, an analysis could be made. A possible use for the cleaned datasets is to see if there are any correlations between criminal activity and geographic (areas with population size, neighborhood quality, location) & socioeconomic factors (income or wealth, occupation, and years of education. 

Sources:
Dataset is owned, maintained and provided by the Chicago Police Department [Via chicagopolice.org].
Dataset is owned, maintained and provided by the City of Los Angeles Police Department [Via data.lacity.org]. 

