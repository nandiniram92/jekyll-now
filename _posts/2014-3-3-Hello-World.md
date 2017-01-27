---
layout: post
title: The best location for a coffee shop using Data Science!
---
# The First Week at Metis - Project Benson!
Just four days into the bootcamp, we were done with our first project- Benson. We were asked to come up with a backstory for a client based on the MTA Turnstile data in New York and come up with a solution for our client based on the data sets.

## The Backstory of our Client - Lets outsmart Starbucks!
Our client is a small generic coffee shop chain who is looking to expand and set up outlets near some of the ideal MTA stations in New York.  The idea is to target the coffee drinking demographic in order to maximize profits during their daily hours. Since the majority of people in New York commute through the MTA stations, the MTA turnstile data is crucial to estimating the conducive locations which would generate maximum revenue. They have requested our team to come up with a solution based on thorough data analysis.
We used the MTA data sets in combination with the U.S Census ACS 5 year estimates data sets to determine the ideal locations based on both the travel and socioeconomic factors.

## Ideal location for a Coffee Shop: factors?
Talking about the best location for a coffee shop, we would ideally look for some of the following factors:
* Close to an MTA Station which is busy during the popular times of a Coffee shop- when people generally hit the coffee shops!
* Someplace with the optimum coffee drinking demographic - Higher per-capita income, Higher concentration of post-graduates,etc.

## Popular Coffee Shop Hours 
  The popular coffee shop hours in New York according to google is between 11 AM and 3 PM.
  
  ![Popular Coffee Shop Hours](http://www.cultureespresso.com/wp-content/uploads/2013/04/CE-overhead-web.jpg)
  
## Ideal Factors for a station
  The station should be highly populated- we would like a lot of people to be exiting the subway station between the hours of 11   AM and 3 PM. Also, there should be suustained growth and an upward trending model.
  
  ![Subway Stations New York](http://assets.nydailynews.com/polopoly_fs/1.1983020.1413985703!/img/httpImage/image.jpg_gen/derivatives/article_750/78939199.jpg)
 
## MTA Subway Station Data Analysis!
 We obtained the MTA Data sets from the website and used the pandas module in Python to convert them into data frames for easy analysis. After munging and parsing the data, we calculated the total exits from each of the stations between 11 AM and 3 PM for two years- 2015 and 2016. 
 
 ![Trafficked Stations](file:///home/nandini/Pictures/stations.png)
 
 We also calculated the stations with the highest upward trending growth in traffic between the two years.
 file:///home/nandini/Pictures/growth.png
 
 We cross referenced both the lists and came up with top 24 stations that would be ideal in terms of traffic.
 file:///home/nandini/Pictures/finallist.png
 
## Census Data Analysis
 To further narrow down on the best possible location for our client, we introduced the demographic perspective and retrieved the census data for every tract in New York through the bureau's ftp server, and then narrowed down the data by geolocating the areas near the filtered stations from the previous analysis. With our census tracts and their proportions within the given radii identified, we were able to pull our chosen metrics from the Census’ API and extrapolate them to accurately reflect the socio-demographic characteristics of those most likely to frequent each terminal.
 
 file:///home/nandini/Pictures/censustract.png
 
 file:///home/nandini/Pictures/censustract.png
 
## Market Research and Final Analysis!
 We analysed the census data that we pulled out, by referencing the market data from Small-Business development Community Network and the Coffee Shop Business Overview report. We allocated the weights to each of the factors in the population description - The Well educated, The High-Earners and the Singles- that have been known to purchase a lot of coffee! We also included a factor to weigh in the competitive angle- taking into account other coffee shops nearby so that our client stands out!
 Voila, here is our final scoreboard!
 file:///home/nandini/Pictures/scoreboard.png
 
 Based on the final results, we presented our client with an accurate visualization of our final scoreboard-
 file:///home/nandini/Pictures/comprehensive.png
 
 
## Our Recommendations- Look out, Starbucks!
 ![Recommendation#1](https://s-media-cache-ak0.pinimg.com/564x/3a/6a/16/3a6a1689241b0ae920e4f2d0160db57f.jpg)
 
 ![Recommendation#2](http://www.brooklyneagle.com/sites/default/files/styles/free_style/public/pages/bay-ridge-86th-street-subway-elevator.jpg?itok=YDlnIQMF&c=188db6c16fadbb041b6fe9d1f2015ed2)
 
 ![Recommendation#3](http://subwaynut.com/irt/utican3/utican38.jpg)
  





