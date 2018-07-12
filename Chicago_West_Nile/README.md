# Project_4

PROBLEM: 
Given weather, location, testing, and spraying data, predict when and where different species of mosquitos will test positive for West Nile Virus within the city limits of Chicago.


OBJECTIVE: 
Build a model and make predictions that the City of Chicago can use when it decides where to spray pesticides.  Conduct a cost-benefit analysis.  This includes annual cost projections for various levels of pesticide coverage (cost) and the effect of these various levels of pesticide coverage (benefit). 


QUESTIONS: 
How would we quantify the benefit of pesticide spraying? To get "maximum benefit," what does that look like and how much does that cost? What if we cover less and therefore get a lower level of benefit?


TEAM MEMBERS:
Gil Medeiros- Team Lead
Zach Cox - Lead Analyst
Jordan Arnold - Data Steward

PRESENTATION: https://docs.google.com/presentation/d/1FuZGRFN7roo9-qT-i9Rn7iMSeTWIC-aW_VOF1GDoIWU/edit?usp=sharing

TIMELINE:
https://docs.google.com/spreadsheets/d/17ExKVwvCxxSEcklkB5acXdMxXPxlzTehUz3HE1rRlC4/edit?usp=sharing


PERSPECTIVE PRESENTATION:
Presentation is geared towards members of the CDC. Some mebers of the audience will be biostatisticians and epidemiologists who will understand statistical models and metrics and will want more information.  Others will be decision-makers, focusing almost exclusively on your cost-benefit analysis.  The objective is to convince both groups of the best course of action in the same meeting and be able to answer questions that either group may ask. Length of presentation is ~20 minutes.


PRELIMINARY INFO:
West Nile Virus is most commonly spread to humans through infected mosquitos.  ~20% of people who become infected with West Nile Virus develop symptoms ranging from a persistent fever, to serious neurological illnesses that can result in death.  In 2002, the first human cases of WNV were reported in Chicago.  By 2004, the City of Chicago implemented a surveillance and control program to prevent WNV still in effect today.

Every week from late spring through fall, mosquitos in traps across the city are tested for WNV.  These results influence when and where the city sprays airborne pesticides to control adult mosquito populations.  By utilizing data science methods, a more accurate method of predicting outbreaks of WNV in mosquitos will help the City of Chicago and Chicago Deparment of Public Health more efficiently and effectively allocate resources towards preventing transmission of WNV.  

This project was originally a Kaggle competition sponsored by the Robert Wood Johnson Foundation with data provided by the Chicago Department of Public Health.  The project uses the Kaggle Leaderboard to keep track of participant scores.  The public leaderboard uses ~30% of the dataset to score an AUC (Area Under Curve) metric.  


ADDITIONAL INFO:
Below is a list of general information regarding West Nile Virus published on the City of Chicago's website:

https://www.cityofchicago.org/content/dam/city/depts/obm/supp_info/2018Budget/2018_Budget_Recommendations.pdf
Grants for Department of Public Health 
Mosquito Vector Prevention Program (2017 grant: $380,000)
Mosquito Vector Prevention Program (anticipated 2018 grant: $530,000)


https://www.cityofchicago.org/city/en/depts/cdph/supp_info/infectious/west_nile_virus_surveillancereports2011.html

2011
West Nile Virus Surveillance Reports Notes

- Mosquitos are most active at nighttime (between dusk and dawn).
- All sources of standing water support mosquito breeding, including water in bird baths, ponds, flowerpots, wading pools, old tires, and other receptacles.  
- If interested, there are weekly reports at this url

https://www.cityofchicago.org/city/en/depts/cdph/supp_info/infectious/preventing_west_nilevirus.html

Preventing West Nile Virus

- Mosquitos like tall grass and weeds
- Many of the mosquitos that carry West Nile Virus bite between dusk and dawn (nighttime)


https://www.cityofchicago.org/city/en/depts/cdph/provdrs/healthy_communities/news/2017/june/city-health-department-encourages-west-nile-virus-prevention.html

June 2017
City Health Department Encourages West Nile Virus Prevention

- People age 50+, with chronic health conditions, and/or compromised immune systems are at greater risk of becoming seriously ill with WNV
- Charateristics of WNV: fever, muscle aches, rash, headaches, significant weakness and fatigue
- on average, only 2 out of 10 people bitten by infected mosquito will actually become ill
- Key to controlling WNV is reducing population of Culex pipiens aka the Northern House Mosquito. They lay eggs in standing waters which are found in almost any environment
- Chicago’s sister agencies are assisting by providing larvicide treatments (90% effectiveness rate) for their agencies, Chicago Park District and Chicago Public Schools

https://www.cityofchicago.org/city/en/depts/cdph/provdrs/healthy_communities/news/2010/aug/city_to_spray_insecticideonwestnwsidetofightmosquitoeswestnilevi.html

August 2010
City to Spray Insecticide on West/NW Side To Fight Mosquitoes, West Nile Virus
- Spraying occurred in the Austin and Belmont Cragin areas where CDPH (Chicago Department of Public Health) traps yielded mosquitos carrying WNV
- Spray occurs ~8pm on Wednesdays with technicians dispensing ultra-low-volume spray.  
- The material being used to control the adult mosquitoes, Evergreen 60-6, will be applied at a rate of 0.87 fluid ounces per acre. It is approved for use by the U.S. Environmental Protection Agency and is used to control mosquitoes in outdoor residential and recreational areas.

Evergreen 60-6 is a natural pyrethrin product. Pyrethrins are a botanical insecticide group produced primarily from chrysanthemum flower extracts. Pyrethrin has been used effectively to control insects for decades and is non-persistent, decomposing rapidly in the environment. This rapid degradation of pyrethrin makes it an excellent choice for control of WNV-carrying mosquitoes.

The spray will be applied by technicians from Vector Disease Control Inc., a leader in the mosquito control industry. Guiding the crews through the streets will be supervisors from the Chicago Department of Streets and Sanitation.

While the spray is not harmful to people or pets and is routinely sprayed in residential areas across the nation, residents of targeted neighborhoods may choose to stay indoors and close their windows while spraying is underway, as an extra precaution.

READ THIS FOR PRICE INFO:
“Spraying to kill adult mosquitoes is a sensible and effective component of an integrated pest management program. We spray when we have clear evidence that the West Nile Virus has made significant inroads into a community,” added CDPH Environmental Health Director Cort Lohff, M.D. “And while no one can control the weather—and in a city of 228 square miles we can't prevent every single mosquito from hatching and biting, it is our expectation that this effort, by further limiting the mosquito population, will prevent cases of human illness in Chicago.”

The Northern House mosquito, Culex pipiens, is the primary carrier of West Nile virus. This mosquito species thrives in water with high organic content, such as that found in catch basins (storm sewers). Consequently, a hot, dry summer increases the risk of West Nile virus infection, exactly the opposite of what many people believe.

In contrast, the swarms of mosquitoes most people currently are experiencing are Aedes vexans, which is a common "floodwater" mosquito that appears after heavy rains. This mosquito may be a nuisance, but they rarely are infected with West Nile Virus. Therefore, although the number of mosquitoes has significantly increased in recent weeks, the risk of WNV transmission outside the current spray zone has not.

- In 2009, 720 (32 fatal) cases occurred of WNV in US, only 1 case in Chicago (non-fatal)
- Sustained presence of virus in Austin, Belmont Cragin, Forest Glen, and O’Hare Airport areas
- Virus detected only sporadically in Dunning, Portage Park, Norwood Park, Chicago Lawn, Clearing, New City, and West Pullman neighborhoods


https://www.cityofchicago.org/city/en/depts/cdph/provdrs/healthy_communities/news/2015/june/cdph-encourages-residents-to-take-precautions-against-west-nile-.html

June 2015
CDPH Encourages Residents to Take Precautions Against West Nile Virus
- WNV cannot be transmitted from person to person.  Only transmitted to humans via mosquitos. Most mosquitos don’t carry the virus


https://www.cityofchicago.org/city/en/depts/cdph/provdrs/healthy_living/news/2010/jun/city_health_departmentannouncesactionagainstmosquitoeswestnilevi.html

June 2010
City Health Department Announces Action Against Mosquitoes, West Nile Virus
- “City’s plan to thwart WNV is aggressive and prevention-oriented”
- Crews are dropping larvicide briquettes down all 210,000 catch basins on the public way.  This prevents large amounts of larvae from developing into biting adults

Final Results: Voting Classifier using SVN, Logistic Regression, as well as a few other weaker models.
ROC-AUC Score 0.65268 which was in the top half of Kaggle Submissions for this project.

Data Dictionary (pre-imputation):
    train.csv, test.csv - the training and test set of the main dataset. The training set consists of data from 2007, 2009, 2011, and 2013, while in the test set you are requested to predict the test results for 2008, 2010, 2012, and 2014.
    Id: the id of the record
    Date: date that the WNV test is performed
    Address: approximate address of the location of trap. This is used to send to the GeoCoder. 
    Species: the species of mosquitos
    Block: block number of address
    Street: street name
    Trap: Id of the trap
    AddressNumberAndStreet: approximate address returned from GeoCoder
    Latitude, Longitude: Latitude and Longitude returned from GeoCoder
    AddressAccuracy: accuracy returned from GeoCoder
    NumMosquitos: number of mosquitoes caught in this trap
    WnvPresent: whether West Nile Virus was present in these mosquitos. 1 means WNV is present, and 0 means not present. 

spray.csv - GIS data of spraying efforts in 2011 and 2013
    Date, Time: the date and time of the spray
    Latitude, Longitude: the Latitude and Longitude of the spray
    
weather.csv -https://www.kaggle.com/c/predict-west-nile-virus/data

Thanks for reading, feel free to reach out anytime at gibert.medeiros8046@gmail.com for questions or comments, I would love any feedback as im constantly trying to expand my knowledge.