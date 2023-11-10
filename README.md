# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This objective is to create a statistical model with python utilizing data sourced from multiple APIs. The APIs used in the process were *Citybikes, foursquare and Yelp.* Marsaille of The Provence-Alpes-Côte d'Azur region in southern France is the city chossen for this analysis.
The goal is to analyze bike ridership in relation to access to local amenities, and to evaluate access and influence of restuarant ratings in proximity of bike stations.

## Process
### Step 1: accessing data
The first step involved requesting data from Citybikes for Marsaille, parsing through data, and creating a a dataphrame for said data. Once Data was parsed, and checked for completion it was saved to CSV for ease of access between notebooks. 

The same process was done for restaurant data within 1000m proximity to very station requested from CityBikes.

### Step 2: Combining data
This step involed more cleaning and ommiting of unneccesary collumns and joining of tables. The goal was to keep the table as simple as possible, since ther would be numerous null values. 
Key values kept within the dataset included:
- Name
- Distance
- Lattitude
- Longitude
- Rating
- Review Count

Duplicate rows were removed, null values were assessed and either removed are mean values were applied to maintain uniformity within dataset.

### Step 3: Analysis
For analysis, a linear regression model was utilized. This model was chosen used to determine a correlation between dependant varialbes (free bikes, distance) and the independant variables. 

## Results
(fill in what you found about the comparative quality of API coverage in your chosen area and the results of your model.)

## Challenges 
staying organized and maintain consistency within my analyisis was a major challenge, as the further I dove within the data, the more imperative it was to stay organized. My exceution of the APIs was flawed, and I made several mistakes which forced me to restart the process a few times and ommite some of my data (foursquare). 
Deciding what data to keep for analysis vs what data tonot include was challenging. Filling in Null values was a major point of contention for me as I felt it would skew the data, but I could not complete the anaysis with them included.

## Future Goals
(what would you do if you had more time?)
