# Chicago crime analysis

## What is your issue of interest (provide sufficient background information)?
   The crime rate is a prevalent concern that is skyrocketing in the USA for many years . For the final project I have chosen a dataset about the crimes in Chicago for    past 2 years, the dataset was pretty interesting as it had real-time information about the crimes happening in Chicago, moreover, the data is updated every day. The    dataset was collected from the ‘city of Chicago’s official website which has many public datasets. 

## Why is this issue important to you and/or to others?
   The main reason why I chose this dataset was because there were many columns which provided a comprehension idea about the dataset and moreover many interesting        patterns and insights can be drawn from the dataset. The main reason why I chose Chicago is that it is considered one of the cities in Illinois with the highest        crime rate.

## What questions do you have in mind and would like to answer?
   1. To investigate the sorts of crimes that happened more often. 
   2. What types of offenses were deemed serious, and whether they were Punished? 
   3. Based on the geographic location of crimes, look for the hotspots where crime occurs more often. 
   4. By using the IUCR dataset and combining the crime dataset to classify the criminal offenses. 
   5. Find out the most common crimes across Chicago.
   
   - These are some of the issue statements that made sense when looking at the data. However, as we gain a better understanding of the data through EDA and analysis,
     there may be additional fascinating patterns and insights through which we might discover more effective problem statements.

## Where do you get the data to analyze and help answer your questions (creditability of source, quality of data, size of data, attributes of data. etc.)?
   https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/data

  The dataset consists of 22 columns and 7.62 million rows (dataset size ~1.78GB). The dataset has information about the reported crimes from 2001 in the city of Chicago except for the murders. The data comes from the CLEAR (Citizen Law Enforcement Analysis and Reporting) system of the Chicago Police Department. Addresses are only published at the block level to preserve the anonymity of crime victims, and individual locations are not revealed.While the dataset has many columns it also has a column called (IUCR) Codes which are basically, Illinois Uniform Crime Reporting codes; these are four-digit codes that law enforcement agencies use to classify criminal incidents when taking individual reports. These codes are also used to aggregate types of cases for statistical purposes. In Illinois, the Illinois State Police establish IUCR codes, but the agencies can add codes to suit their individual needs. The Chicago Police Department currently uses more than 400 IUCR codes to classify criminal offenses, divided into “Index” and “Non-Index” offenses. Index offenses are the offenses that are collected nationwide by the Federal Bureaus of Investigation’s Uniform Crime Reports program documents crime trends over time (Data released semi-annually), and include murder, criminal sexual assault, robbery, aggravated assault & battery, burglary, theft, motor vehicle theft, and arson. Non-index offenses are all other types of criminal incidents, including vandalism, weapons violations, public peace violations, etc. I am not sure whether I will use this particular dataset in-depth or not however in the case of use I would like to attach the link for this dataset as well.

## What will be your unit of analysis (for example, patient, organization, or country)? Roughly how many units (observations) do you expect to analyze?
   Crimes
   Community Area
   Latitude
   Longitude


## What variables/measures do you plan to use in your analysis (variables should be tied to the questions in #3)?
   - Date - Date on which crime occured. 
   - Primary Type - Primary type of crime.
   - IUCR - Four digit Illinois Uniform Crime Reporting (IUCR) codes
   - Description - Short description of the type of crime
   - Location description - Description of where crime occured
   - District - District code where crime occured
   - Community - Community area code where crime occured
   - Longitude & Latitude - Exact coordinates of crime occurance
   - FBI Code - numeric code indicating FBI crime categorization
   - Year - Year of crime
   - Arrest - Indicates whether arrest was made or not


## Techiniques:
   * Determining correlation amongst variables for feature selection.
   * I would like to implement classification algorithms such as Logistic Regression, Decision Tree, Support Vector Machine, KNN classifier, Random Forest to predict        Primary Type of the crime.
   * The KNN Classifier is effective at making real-time predictions. It is critical that all features be scaled to the same level. As a result, when building a model      with KNN, we will employ the standard scalar technique.
   * Implementing grid search for optimal parameter selection.
   * Creating an ensemble model, such as Random Forest, to reduce variance in the data. If there is a chance of overfitting, Random Forest will perform well with the        data. Because the data contains many categorical values, working with Random Forest would be a better option.
   * Determining confusion matrix, accuracy score, RSME value and other support metrics such as precision recall and F1.
   * Finally, I would like to develop a webpage which takes the location as input and gives the crime rate at that particular location which can help people looking        for a house in that specific location.
