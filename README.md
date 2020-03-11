# Analysis of CitiBike program, NYC, July - December 2019

The purpose of this proejct was to analyze Data from the CitiBike using tableau. The data was extracted from the CitiBike data website, combined and saved as a single CSV file using Python libraries pandas, numpy, requests, zipfile, io and glob. Analysis of the data was completed in tableau. 

## Analysis

### Demographics

#### The rate of change of each Gender and Age Range demographic tends to be similar to each other 

##### Gender

While among riders whose gender is known, CitiBike rides are more frequently ridden by by males, when the total overall number of rides increases, the percentage increase of rides for both Male and Female riders tend to be similar. The same is true when the number of rides decline. 

This means when the total number of rides increases, the share of rides taken by Males increases. 

If there is any effort to increase the number of Female riders, the specific efforts should be re evaluated because they do not appear to be effective. The lack of Female ridership may indicate an untapped market for potential future growth. Future marketing efforts can be targeted to potential Female riders by highlighting the benfits that a Female rider may see, and these marketing efforts should be concentrated in mediums in which potential Female riders have a higher likihood of seeing or hearing the advertisement. 

##### Age Range

Similar to the above, among riders whose ages are known, the rate of change for each age group tends to rise and fall at similar rates to eachother. The only exception to this is that CitiBike riders who are teenages was nearly flat the entire period. 


### Extreme Rental Lengths

#### Greater than one day

Standard CitiBike rides can last up to 30 minutes, and rides for annual membership holders can last up to 45 minutes without incurring steep additional fees. The additional costs associated with keeping a CitiBike rented for a day without returning it can exceed the annual cost of an 'unlimited' membership, in which a customer can rent a CitiBike as many times as they want 45 minutes at a time. This gives a clear financial incentive for a customer to return their rented bike within 45 minutes, even temporarily if they intend to ride for longer than 45 minutes. 

There is a high prevalence of CitiBike rentals exceeding one day (86,400 seconds, the unit of measure for rentals). At approximately 2,900 over the six month period analyzed, approximately 16 rentals per day on average were rented for longer than a day. The ending station of these rides is diverse. Except for a handfull of bikes that have three or four rentals exceeding a day, the CitiBikes that have rentals exceeding a day only have one or two over the 6 month period analyzed. 

The diverse ending stations should rule out this being caused by faulty equipment at the ending station. The samll number of rentals per bike, along with anecdotal instances of CitiBikes being rented shortly after the long rentals end, should rule out faulty equipment on the bikes, or bikes needing repairs. 

Additional data is necessary to understand why there are so many long rentals. It may be useful to look at communications from or with customers with rentals exceeding a day. 


### Popular Starting Stations, Morning Rush Hour

During the morning rush hour, between 6 and 9 AM, the most popular starting stations tend to be in New York City, south of Central Park. These riders are likely commuting to work to locations that do not require the rider to cross a bridge or tunnel. The housing costs in Central Park inside New York City implies the income level of those living in this area may be high enough such they those living in this area may be able to afford more expensive modes of transportation.

## Dataset

1. Can be located at: https://www.citibikenyc.com/system-data

## Final Files

The final tableau notebook is located in citibike.twb and to obtain the data I used, you need to run all the cells in the combineCSV_and_cleanData.ipynb jupyter notebook. 
