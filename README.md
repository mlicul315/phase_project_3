# Seattle Terry Stops
Author: [Michael Licul](mailto:liculm315@gmail.com)
![Screenshot 2023-01-09 at 3 57 16 AM](https://user-images.githubusercontent.com/97541858/211273123-bb3e589e-85c1-48f6-9c3f-3ffa35428fb0.png)

## Overview 
Terry Stops permit law enforcement to detain an individual based on reasonable suspicion of a crime. In 1967-1968 the Supreme Court case, Terry v. Ohio, the court ruled that stopping an individual on suspicious behavior does not violate the ‘unreasonable search and seizure’ clause of the Fourth Amendment. Thus, Terry Stops were born. 

As an independent data scientist, my goal was to analyze Terry Stops that ended in an arrest. I analyzed Terry Stop data from the Seattle Open Data database.  I looked over 50,000 cases of Terry Stops between 2015-2022 and built a model that predicts the likelhood a person will be arrested with 83% accuracy. While I ran multiple models and tuning each models parameters, the model with the highest accuracy score was the Gradient Booster Model. It performed better than the Logistic Regression, Random Forrest, and Decision Tree models. 

## Buisness Case
As an independent data scientist, my goal was to analyze Terry Stops that ended in an arrest. I analyzed Terry Stop data from the Seattle Open Data database. I looked over 50,000 cases of Terry Stops between 2015-2022 and built a prediction model to based on the data. My target audience was the Equal Justice Matters. Founded in 2020, Equal Justice Matters aims "to make an impact by highlighting disparities and inequities within the U.S. Justice System."  Therefore, by focusing on what factors may lead to an arrest, Equal Justice Matters can pursue policy change reagrding the issue. 

![Terry v. Ohio](https://img.geocaching.com/waymarking/display/e6a132fc-7cdf-4ceb-b337-abb23672907f.jpg)

## Data Understanding 
Columns: 
   - [Subject Age Group]: Subject Age Group (10 year increments) as reported by the officer
   - [Stop Resolution]: Resolution of the stop as reported by the officer
   - [Weapon Type]: Type of weapon, if any, identified during a search or frisk of the subject
   - [Officer YOB]: Officer Year of Birth
   - [Officer Gender]: Gender of the Officer 
   - [Officer Race]: Race of the Officer
   - [Subject Perceived Race]: Race of the Subject 
   - [Subject Perceived Gender]: Gender of the Subject 
   - [Reported Date]: Date the stop was reported
   - [Initial Call Type]: Initial classification of the call as assigned by 911
   - [Final Call Type]: Final classification of the call as assigned by the primary officer closing the event
   - [Arrest Flag]: If a physical arrest was made 
   - [Frisk Flag]: If a "frisk" was conducted 
   - [Precinct]: Precinct of the address associated with the underlying Computer Aided Dispatch (CAD) event

## Data Cleaning
Since I am looking at Terry Stops that resulted in an arrest as the target feature, I classified the 'Stop Resolution' columns into two categories:
   - 0 = No Arrest 
   - 1 = Arrest

Additioanlly, I created bins / and combined values in different columns to make better visuals. These included: 
   - Officer Age from Officer YOB
   - Officer Age Group
   - Time of Day
   - Subject Percevied Race
   - Officer Race
   - Combined Weapon Types


## Exploratory data analysis
After the data was cleaned I built several visuals to get a better understanding of what I was looking at. 
### Outcomes
![download-2](https://user-images.githubusercontent.com/97541858/211276103-e7546229-fc37-42f2-ac2b-9cc78c643f84.png)
By looking at the visual, there are various outcomes.
- Field Contact: ~42%
- Offense Report ~31%
- Arrest: ~25%
- Referred for Prosecution & Citation / Infraction: < 5%

### Arrest by Year
![download-1](https://user-images.githubusercontent.com/97541858/211276313-018f2ef1-9d10-4c41-900a-5283e67b3264.png)
The 'Arrest by Year' visual results show:
- Year with Most Arrest: 2018 with ~2300
- Year with Fewest Arrest: 2022 with ~950
There was a drastic decrease in arrest between 2019 and 2020. Arrest continue to decrease up until the data ends in 2022.

### Arrest by Weapon Type
![download](https://user-images.githubusercontent.com/97541858/211276425-18c5cbdf-3e50-4eb6-8963-e9de43e91df4.png)
The 'Arrest by Weapon Type' visual shows:
In ~90% of arrest, no weapon was reported to be found on the subject.
I intended to drop the remaining columns aside from 'Cutting / Stabbing Instrument', but I wanted to keep them on the visual to show the staggering difference between any weapon found and no weapons found.

## Predicitve Model 

## 
