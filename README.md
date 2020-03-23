# ckme136

# Exploring Relationships between Opioid Prescriptions and Opioid Overdose-related Fatalities in the United States of America

# Datasets 

The Centres for Medicare & Medicaid (CMS) in the United States of America (USA) is the agency within the U.S. Department of Health and Human Services (HHS) that administers the nation’s major health care programs [12]. CMS provides open information on drug prescriptions across the USA. A subset of data from CMS was posted to Kaggle [13]. This dataset contains summaries of prescription records for 250 common opioid and non-opioid drugs written by unique licensed medical professionals in 2014 in the United States for citizens covered under Class D Medicare as well as some metadata about the doctors themselves. This dataset had been cleaned and compiled with 1 row per prescriber and limited the approximately 1 million total unique prescriber to 25,000 to allow for better management of the dataset.
3 datasets are included in this package related to prescriber types, opioid types, and opioid-related drug overdose fatalities.

Kaggle - https://www.kaggle.com/apryor6/us-opiate-prescriptions

Three Datasets:

1. Prescribers

The data consists of the following characteristics for each prescriber:
•	National Provider Identifier (NPI) number
•	Gender (M/F)
•	State – U.S. State and Territory by abbreviation
•	Credentials – Set of initials indicative of professional healthcare-related degree
•	Specialty – Description of type of medical practice
•	A list of drugs with numeric values indicating the total number of prescriptions written for the year by that individual prescriber
•	Opioid.Prescriber – a Boolean label indicating whether or not that individual prescribed opioid drugs more than 10 times in the year

2. Opioids

List of drugs classified as Opioids – both Drug Name and Generic Name. There are 113 entries in total. This dataset can help extract opioid-related prescriptions from the Prescribers dataset – as both opioid and non-opioid prescription medications are included in that dataset.

3. Overdoses

This dataset provides statistics on opioid-related drug overdoses in 2014.
It contains the following columns:
•	State – U.S. State 
•	Population – Population levels in each U.S. State 
•	Death - # of opioid-related drug overdoses in each U.S. State
•	Abbrev – U.S. State abbreviated


Step 1: Explore trends in opioid prescriptions
The Opioids dataset will be used to pull out opioid prescriptions from the Prescribers dataset.
I will examine whether particular opioids are prescribed more than others, and whether there are particular opioids that are often co-prescribed with other medications.
This will provide information about the general trends in opioid prescriptions within these datasets.

Step 2: Explore trends in prescriptions from healthcare professionals
I will use the Prescribers datasets to gather more information on the healthcare professionals that are prescribing such opioid medications.
I will examine trends on whether particular types of healthcare professionals are prescribing more opioid medications than others, and whether this varies by U.S. state.

Step 3: Develop a predictive model between opioid prescriptions and overdose fatalities
Finally, after gathering information from exploring information related to opioid medications & healthcare professionals that prescribe such compounds, I will aim to develop a predictive model (e.g., regression analysis) between opioid prescriptions and opioid-related overdose fatalities. 
