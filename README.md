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


## Exploratory data analysis
A 

## Predicitve Model 

## 
