# Data Information
- There are three data sets from the original paper:
  1. The main data set, main_data.csv, consists of data scraped from Airbnb and responses from hosts. There are 7,554 observations in this file. Each observation consists of a guest name, a host ID, the response given in this guest/host interaction, and a series of host and location characteristics scraped from Airbnb. This data set also has classifications for the host's race, gender, and age. These are taken from Mechanical Turk surveys.
  2. The second data set comes from a survey where we asked people to classify the names in our study as "white" or "African-American." This data set is entitled name_survey_results.xlsx. It consists of 24 observations, each of which is a name and a rating from 1 to 2, with 1 being African-American and 2 being white. The rating is the average rating given by survey-takers for each name.
  3. The third data set is hosts.dta. This data set has one observation per host, for a total of 7,594 observations.  This data set includes information on the racial makeup of the host's past guests. 

- The original data is found in the raw_data folder.
- The cleaned data (after replicating the cleaning process from the original analysis) is found in the clean_data folder.
  - `main_data_cleaned.csv`: the main data cleaned according to the original analysis before merging with other datasets
  - `survey_data_cleaned.csv`: the survey data cleaned according to the original analysis before merging with other datasets
  - `merged_main_survey.csv`: the main data and survey data merged with additional cleaning (including new columns such as "yes" which identifies if a host accepted the booking)
  - `merged_with_hosts.csv`: the above dataset (merged_main_survey.csv) with hosts data merged into it