# Communicate-Data-Findings
## by Suryaday Nath

## Dataset

> The Ford Go Bike data (now Bay Wheels' trip data) is a comprehensive and very neatly designed dataset. It provides users to explore various facets of the usage detail and statistic of the data related to bike rentals.

These data were collected efficiently, providing valuable data gathering to work with and draw conclusions.

This Notebook uses data gathered between January 2018 and December 2018. Roughly 1,850,000 bike rides is registered in the San Francisco Bay area of California , USA.

The Original Data:

Each trip is anonymized and includes:

	-Trip Duration (seconds)

	-Start Time and Date

	-End Time and Date

	-Start Station ID

	-Start Station Name

	-Start Station Latitude

	-Start Station Longitude

	-End Station ID

	-End Station Name

	-End Station Latitude

	-End Station Longitude

	-Bike ID

	-User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)

	-Bike_Share_for_all_trip
	
> The following columns were added to the dataset:

	-Start Time Month

	-Start Time Day

	-Start Time Hour

	-End Time Month

	-End Time Day

	-End Time Hour

	-Distance (miles)

	-Duration (Mins)


## Summary of Findings

1. There is a distinct pattern observed among the different type of users of the rental service especially between Customers and Subscribers from which we can speculate about the demographics of the users. 

2. It can be seen that most number of Subscribers travel a distance concentrated within 0.4 to 0.6 miles and 0.8 to 0.9 miles range. 

From the previous plot of duration mins, it can be speculated that the demographics of Subscribers may be a mix of:

a) Office goers and students who use the bikes for convenience - shorter distance travel between the nearest train station perhaps to the office or school. 

b) Tourists with subscription who use the bikes more casually to explore the area. 

While for Customers it can be seen that their travel is distributed across all distances. What is unique about this distribution is that a huge number of customers are travelling within 0 to 0.1 miles. 

Thus, one implication of this observation might be that Customers are using the bikes more leisurely than Subscribers.

For Bike share for all scheme users, they are renting it for lesser duration and also riding it for less miles i.e. 0.4 to 0.6 miles comparatively. It might imply that they are using the bikes for day-to-day usage or tasks. 


3. There is a stark difference between the start hour of rentals for Customers and Subscribers. Start hour of rentals peak during the later part of the day and towards evening for Customers.

Start hour of rentals for Subscribers follow the pattern where peak timings are between 7-9 and 4-6 in the evening. Which are usually office and school starting and ending hours. Which again points to the fact that Subscribers may be mostly office goers and school kids and Customers may be travellers.

4. The pattern for months seem to show that months May-October being the months which see the most number of rentals with the peak for Customers on July and for Subscribers on October.

For Customers, demand peaks for July which sees good weather and demand wanes off during September, October (maybe because the region sees the highest temperature during that time and there aren't many travellers).

October is one of the busiest months in San Francisco because of a multitude of events and attractions during that time and maybe the company sees a lot of conversions from Customers to Subscribers during that time.

5. Looking at the violin plots reveal that customers rent the bikes over a wide variety of ranges and for about 7.0 to 12.5 minutes on average while for Subscribers, there seems to be a large number of people per time duration for almost every duration as there are spikes during different durations.

 5. It is seen that the distance travelled by Customers and Subscribers are similar except that for Subscribers, there are far more outliers than Customers meaning Subscribers travel more distance overall than Customers.

6. The top 2 locations of rentals for Customers sees a huge influx of Customers. A quick Google search reveals that the top 2 locations are very well known tourist locations which sees a large number of tourists and it is a popular place of hangout for kids and adults alike. .

7. The top few locations are very different from the Customers locations. The first 2 locations for example seem to be train stations which is used by people to commute. Maybe Subscribers who come to these stations from different locations rent bikes here to commute to nearby schools or office. Again, this is a speculation which can be confirmed by other studies but, it is not within the scope of this project.

8. It can be seen that initially for increase in Rental duration, the distance in miles travelled by Subscribers increased but eventually as the rental duration increased, there is no visible increase in Distance travelled. Which means that subscribers are travelling more distances in short duration or they are renting for long durations and trvaelling short distances.  

9. Subscribers seem to be renting the bikes during weekdays mostly (office and school days) with the exact same pattern of start hour every day (office or school hours). 

During Saturdays and Sundays, demand wanes off with very few Subscribers renting the bikes compared to weekdays and also the start hour seem to start late than usual. 

So, Subscribers can very likely be office goers and students and tourists who subscribed to the plan. 

10. For Customers, during weekdays, the start hour starts late for rentals compared to Subscribers. During weekends, demands peaks and is much more compared to weekdays. The demand peaks in the afternoon and continues on till evening. 

So, Customers may be tourists in that area. 


## Key Insights for Presentation

1. In the presentation, we will be looking at the plot of distance travelled by different users which seem to show a pattern as to the demographics of the user. 

2. We will further explore this theory by looking at the start months and start hour of rentals for Customers and Subscribers. 

3. Then we will dive into more detail using Multivariate exploration wherein we will look at the distribution of start day and start hour for both users in a facet grid and more visibly through a Heat map. 