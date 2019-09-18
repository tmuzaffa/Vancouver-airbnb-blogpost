# Vancouver-airbnb-pricing trends for  most popular neighbourhoods-blogpost
![png](0.png)
###  A review of the Vancouver's air bnb data-UDacity-CrispDM Project

#### BUSINESS UNDERSTANDING

The data sets obtained for the analysis of  vancouver air bnb market contain property listing data set, calendar data set, and reviews data set. All these data set gives us insights about the Vancouver air bnb market. We will use these data set in tandem to find corrleations and answer the following questions.  

Pricing correlation:
* How does price correlates with seasons of year?
* How the type of property impacts the listing price in Vancouver??
* Dependance of listing price on the neighbourhoods in Vancouver?



Analysis of Reviews:
- Understanding how reviews impact the occupancy rate
- Get a correlation of the reviews with the neighbourhoods in vancouver
- Can we explore some of the worst reviews for additional insights?


Influence of parameters on availability:
- Cancellation policy
- Room type
- Number of guests
- Guests picture





    

### Data set review

Now we look at all the data sets to find their characteristics and if they have null values, we will is.null() functionality to check the missing values and will use the .describe() to get some sense of features for each column.

Questions to be answered for data review
1. Are there any missing values?
2. What are the features of each column?


Below analysis show that the vancouver hosts respond very efficiently


![png](output_20_0.png)


It can be seen that approximately 70% of the hosts in metro vancouver respond with in an hour. There are various types of properties available in Vancouver in the Air bnb platform. Below is the breakdown


![png](output_24_0.png)

Approximately 35% of the properties listed on Vancouver Air bnb are houses and 26% are apartments

### Question 1 - Price correlations
1. Understand the correlation between price and the season of the year, and detect the peak season in Vancouver
2. To get an understanding of price correlation with the neighbourhoods in vancouver
3. Getting an insight into the relationship between the listed pricing and the property type in metro vancovuer




![png](output_29_0.png)

July-September seems to be the peak season in Vancouver




![png](output_30_0.png)


As we can see that listing price is higher for the number of reviews between 200-300, as the number of reviews increase we can see that price drops, which suggests that more customer tend to review places which are economical, however places with 200-300 tend to have higher listing price. 

Now we look at the neighbourhood and their pricings




    


![png](output_32_1.png)





![png](output_33_0.png)






![png](output_34_0.png)





It can be seen from the charts above that the highest average price listed per night is $250 and cheapest is $120 per night in metro Vancouver.





![png](output_40_0.png)



It can be seen from the heatmap above that Houses in downtown Vancouver area have higher listing price than apartments. 


### Question 02 - Review correlation

- Understanding how reviews impact the occupancy rate
- Get a correlation of the reviews with the neighbourhoods in vancouver
- Can we explore some of the worst reviews for additional insights?

let us look at the data in the review and listing table and also calcualte the occupancy rate from the listing can calendar table


![png](output_48_1.png)



Review rates are higher for properties with high occupancy rate. This could be either bad review or good review



![png](output_57_0.png)






![png](output_59_0.png)


### Question # 03

Now we will look at the influence of parameters such as below on the availability rate 
- Cancellation policy
- Room type
- Number of guests
- Guests picture


First we try to clean the data and deal with the missing values, For bathrooms column, there are two missing values, but a property must have atleast 1 bathroom, so we will use 1 to fill the NA. We will also drop unnecessary columns






![png](output_74_1.png)








![png](output_77_1.png)


##### Results

Botique hotels are the least occupied property in metro vancouver


``




![png](output_80_1.png)







Above results suggest that, properties with more moderate to flexible cancellation policy tend to have more demand and higher occupancy, whereas properties with more strict cancellation policy have more availability. This suggests that for higher profits, businesses should move towards more relaxed cancellation policy





![png](output_83_1.png)




Listings which can host from families upto a small group are high in demand







![png](output_86_1.png)




Properties that donot require guests profile photo for booking  has low availability and are more popular

