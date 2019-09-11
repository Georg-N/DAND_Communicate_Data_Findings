# Flights dataset
## by Georg Nicola


## Dataset
This dataset reports flights in the United States, including carriers, arrival and departure delays, and reasons for delays. I have chosen the data of the year 2008, which is the most recent available year. The data can be found under the link http://stat-computing.org/dataexpo/2009/the-data.html


## Summary of Findings

Main Findings:
- The amount of flights seems to decrease towards the end of the year.
- The amount of flights is fairly distributed over the days of the month. It makes sense that the 31 has less flights as not every month has 31 days.
- The days Monday to Friday are fairly even distributed. There is a clear drop on Saturday though. Sunday is also below the number of flights during the week but still higher than Saturday.
- Both the arrival and departure time are very low between 1 am and 5 am. Then both pick up, whereas the arrival occurrences go up first then the departure occurrences follow. Therefore, the histogram for the arrivals is overall shifted to the right versus the departure histogram. This behaviour is as expected, as the flights first depart and arrive later.
- The histogram of the elapsed time is unimodal and skewed to the right. The most frequent elapsed times are between 1 and 2 hours. flights higher than 7 hours are very rare, which makes sense as we are looking at US domestic flights.
- Interestingly there is a very high amount of early departures. The amount of early arrivals is rather spread out than the early departures. The delayed departures and arrivals are almost evenly distributed.
- The airline with by far the most flights is WN (Southwest Airlines) from all of the 20 different airlines.
- The overall delay quota is 42.5 % which seems quite high. However any delay bigger than 0 minutes is considered here. The delay categories do not sum up to the total quota, as not for all delays the delay of these categories have been provided.
- As expected there seems to be a correlation between departure delay and arrival delay. However it can be seen that many points are above the red line (which has a slope equal to 1). That means that once the departure was delayed the arrival tends to be delayed even more. In my opinion this is unexpected as I assumed that delays can be caught up during the flight. A possible explanation for this is that an aircraft that is delayed in it's departure cannot get it's original timeslot in the arrival and therefore, gets even more delayed. One has to be careful with conclusions from this plot as the dots are highly overplotted. I will further investigate on this.
- As for the airports with a low number of flights the delay quota is spread out. For the airports with a higher amount of flights the delay quota is between 30% to 60%. The higher the flight frequency the less the spread of the delay quota.
- Even though according to the dots it seems that lower elapsed time causes less delays in arrival the regression line suggests that there is a positive correlation between these two. This positive correlation is very low however. This leads to the conclusion that there is only a minor influence of the actual elapsed time on the arrival delay.
- Apart from the two carriers with the lowest frequency on the left all the other carriers have an average delay ranging from 10 min per flight to 19 min per flight. There seems to be no relationship with regards to amount of flights per carrier and average delay per flight.