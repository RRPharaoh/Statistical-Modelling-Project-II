# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This objective is to create a statistical model with python utilizing data sourced from multiple APIs. The APIs used in the process were *Citybik, foursquare and Yelp.* Marseille of The Provence-Alpes-Côte d'Azur region in southern France is the city chosen for this analysis.
The goal is to analyze bike ridership in relation to access to local amenities, and to evaluate access and influence of restaurant ratings in proximity of bike stations.

## Process
### Step 1: accessing data
The first step involved requesting data from Citybik for Marseille, parsing through data, and creating a data frame for said data. Once Data was parsed, and checked for completion it was saved to CSV for ease of access between notebooks. 

The same process was done for restaurant data within 1000m proximity to very station requested from CityBik.

### Step 2: Combining data
This step involved more cleaning and omitting of unnecessary columns and joining of tables. The goal was to keep the table as simple as possible, since there would be numerous null values. 
Key values kept within the dataset included:
- Name
- Distance
- Latitude
- Longitude
- Rating
- Review Count

Duplicate rows were removed, null values were assessed and removed. mean values were applied to maintain uniformity within dataset.

### Step 3: Analysis
For analysis, a linear regression model was utilized. This model was chosen used to determine a correlation between dependant variables (free bikes, distance) and the independent variables. 

## Results
When it came to the API, I was only able to gather data from Yelp, so might data set might be limited in scope, but the availability of amenities seems to be high as there were over 1846 result to 186 bike stations, which is an average of 9.9 restaurants within a 1000m radius of any bike station. 

Utilizing our regression model, the adjusted R-squared is very low (0.001) which indicates that the model is not giving us any meaningful explanation or correlation between the free bikes, number of ratings and the ratings of restaurants. I then went on to experiment with other values form my dataset, with little success. Some graphs looked to indicate some correlation, but when tested against the linear regression model, the R-squared values were consistently just as low as my original model.

The results prove that my analysis is inconclusive in proving a correlation between the restaurant ratings and their proximity to bike stations. However, this does not mean that there isn't a relationship, it may just mean that I need more data.

## Challenges 
staying organized and maintain consistency within my analysis was a major challenge, as the further I dove within the data, the more imperative it was to stay organized. My execution of the APIs was flawed, and I made several mistakes which forced me to restart the process a few times and omit some of my data (foursquare). 
Deciding what data to keep for analysis vs what data to not include was challenging. Filling in Null values was a major point of contention for me as I felt it would skew the data, but I could not complete the analysis with them included.

## Future Goals
I would like to compare the results of Marseille, with another city of similar size. 
I would also like to investigate additional data that might indicate what the trends in the city are regarding bike usage, for example:
 - is it a walkable city
 - Public Transit accessibility 
 - City policies
 - availability of bike trails.

