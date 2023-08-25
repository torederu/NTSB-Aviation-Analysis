An Exploratory Data Analysis of Airplane Incidents


The Business Problem


As we expand our business into new industries in order to diversify our portfolio, we encounter a few challenges along the way. To be specific, we’re now examining the potential of the aviation sector, but a lack of knowledge of the risk factors has been preventing us from moving forward.


One of our company’s foremost principles has always been that the best way to make money is not to lose it. Therefore, by minimizing the risks associated with aircraft, we can rest assured that this new wing of our portfolio will meet the expectations of the investment.


Specifically, we’d first like to know, which aircrafts are the safest? But what do we mean by “safe?” We want to choose aircrafts that weren’t involved in incidents where the plane was completely destroyed. And if they were (which unfortunately is sometimes inevitable), which of them were able to keep their passengers as safe as possible?


Additionally, we are not solely looking at airplanes as part of this investigation. Helicopters will also be analyzed to determine their safety.


Once we’ve filtered the safest aircrafts, we want to dig into their purposes. What were they made for or what do they specialize in? With that information at hand, we can establish a clear business plan within our parameters.


Lastly, based on our findings, are there certain periods of time or weather to avoid? Minimizing risk might imply creating a seasonal business; if that’s the case, when should we fly?




The Dataset
The data used for this research is from a dataset from the National Transportation Safety Board. This dataset includes aviation accident data from 1962 to 2023 about selected incidents in the United States and across international waters.
The dataset comes in the CSV format, and has 90348 Rows and 31 columns, only one of which showed no null values, with 609971 cells being NaNs in total, which is around 21% of the total dataset.
  
  

Methods
This project involved cleaning the datasets to discover valuable insights into which aircraft models are the safest. We started by standardizing the names of makes and models, then filling or dropping nulls based on the need of that specific cell. We were then able to establish survival and injury rates for each incident.


Afterwards, we created two different algorithms to determine which make performs better overall. A “Damage Index” assigns a score to each incident and its intensity, adjusted by the amount of incidents overall per each make. Second, a set of established filters will evaluate the performance of the plane in each incident, based on the aforementioned survival and injury rates.


Results
Based on the methods explained above, we were able to filter the top performers of all the makes listed using the Damage Index:




* Per the Damage Index, the top makes are: ____________ . These are the companies and brands that are less likely to be involved in an incident in which the aircraft is totally destroyed or suffers substantial damage. However, this doesn’t mean that they’re the safest overall should an incident occur; for this reason, we defer to the second algorithm, the performance model:




* With this model, we can conclude that out of the three makes that we’re observing, the one that keeps the most passengers safe is ______ 
* With a greater % of our passengers safe and uninjured, we can make sure that even in those accidents in which the aircraft suffers great damage, we can minimize the potential human losses and financial penalties in the form of lawsuits.


After we’ve found that ____ is the best performing make, we evaluate the main purposes for which the aircraft is being used, in order to determine the secondary business within the aviation business that this branch of our company will focus on:




* Most of the ___ planes/copters are used for ___, making them the safest choice for business purposes.


For the final note, we needed to see if the weather and time of year has a direct affect on the performance of our top chosen aircraft, in order to further evaluate if it’s wise to run it all year long regardless of weather conditions.




Recommendations
* Planes/copters from the makes: ______ tend to have a minor occurrence of severe accidents.
* WEATHER CONDITIONS
* MONTHS


Next Steps
* While the data available can give us an understanding of how aircrafts perform within certain kind of circumstances, is important to note that this Dataset only includes occurrences in which there were accidents. Therefore, it is not possible to accurately  determine the rate of said occurrences from the amount of times the specific plane was in the air.
* With more time, we could’ve given a breakdown of all
* Collect additional data about




1) Damage index for all makes
2) Performance for all makes, but add a filter so that we can show performance for the top 3 makes only
3) Performance for the top 3 models in each of the top 3 makes 
4) Percent injured (or number of incidents) over time (months), split by weather condition - but only for the top 3 makes 
5) Maybe a bubble chart for purpose for the top 3 makes - for this one I think we might need to manually look up what each plane is for to get more info. Like we looked one up and saw its a touring plane, which is more info that just "personal" which is what the df days