## Query to Rank the count of landing outcomes (such as Failure (drone ship) or Success (ground pad)) between the date 2010-06-04 and 2017-03-20, in descending order.

%sql select Date, Landing_Outcome, count(*) as frequency from SPACEXTABLE where substr(Date,0,10) >'2010-06-04' and substr(Date,0,10) <'2017-03-20' group by Landing_Outcome order by frequency desc

## Query to list the records which will display the month names, failure landing_outcomes in drone ship ,booster versions, launch_site for the months in year 2015.

%sql select substr(Date,6,2) as Month,substr(Date,0,5) as Year, Booster_Version,Landing_Outcome,Launch_Site from SPACEXTABLE where substr(Date,0,5)='2015' and Landing_Outcome like '%Failure%' 


## Query to list all the booster_versions that have carried the maximum payload mass, using a subquery with a suitable aggregate function.

%sql select Booster_Version,PAYLOAD_MASS__KG_ from SPACEXTABLE where PAYLOAD_MASS__KG_=(select max(PAYLOAD_MASS__KG_) from SPACEXTABLE)
