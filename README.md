## Short Description

In this project, I used The Guardian API to search for any articles that mentioned protest over the past year, which resulted in retrieving the titles and urls for 3,000 articles. I used these urls to retrieve the full html text of the articles from The Guardian website. 

I then used a list of country names and assigned a country to each article based on the number of times the country was mentioned in a given article. The country with the max number of mentions was assigned to the article. 

I analyzed this data to find that just over half of the articles mentioned a country at all, bringing my n to roughly 1,500. I also made a frequency table and bar chart that showed the prevelence of reporting on protest by The Guardian over the past year, with the vast majority mentioning Australia and the second highest number mentioning the United States. 

I sorted the countries into regions of the world in order to make the data more easily comprehendable. 

I then created two dictionaries as csv files - one that is meant to capture words that associate protests with being spontaneous expressions of anger and one that is meant to capture words that associate protests with planned and constructive expressions of political engagement. 

I tallied the presence of these words in each article and generated data that showed the counts of what I call angry versus joyful protest reported for each region of the world over the past year. 

The results showed that the prevelence of emotion words - both angry and joyful - were positively rather than negatively correlated, with the most emotion-laden text occuring for Sub-Saharan Africa and North America. 

This project resulted in significant learning, which I am incorporating into a future study. I have obtained articles from the New York Times and Washington Post dating back to 1995 that have been manually tagged as having to do with "protest and demonstration" and which are also tagged by location. I will add additional major international news sources in the United States to this dataset. I believe that focusing on US-based international news sources for a longer period of time that also have manual tagging will provide me with a firmer ground in terms of data. 

Once I have completed this data collection, my plan will be to do topic modeling with this data as a way of understanding regional or international biases in reporting on protest. This may be more beneficial than creating my own dictionary, as my hypothesis failed to show the negative correlation I expected. As a result, I believe topic modeling will be a helpful way of letting the data "speak to me." While this is a long process the work I have done in this first iteration is a promising start. 

## Dependencies

List what software your code depends on, as well as version numbers, like so:.

1. Python 2.7, Anaconda distribution.


## Files

### Data

1. 01_guardiandata.csv: 365 days worth of raw data of articles from The Guardian website. 
2. 02_anger_dictionary.csv: Dictionary I created with words related to spontaneous angry protest. 
3. 03_joyful_emotions.csv: Dictionary I created with words related to organizad constructive protest. 
4. 04_guardian_emotion_data.csv: processed guardian dataset with title, article content, country, and a count variable for anger and joy.

### Code

1. 01_collect_guardian.ipynb: Collects data from The Guardian and exports it to the file guardiandata.csv
2. 02_text_counts_guardiandata.ipynb: Loads and cleans Guardian data and performs counts based on country and emotion dictionaries. 
2. 03_analysis_guardiandata.ipynb: Conducts descriptive analysis of the data, producing the visualizations found in the Results directory.

### Results

1. 01_countries_assigned.png: A pie chart showing the number and percentage of articles assigned to a country. 
2. 02_region_count_bar.png: A bar chart showing the number of articles observed in each region of the world. 
3. 03_anger_count_bar.png: A bar chart showing the count of spontaneous/anger protest words in each region of the world. 
4. 04_joy_count_bar.png: A bar chart showing the count of organized/joyful protest words in each region of the world. 
5. 05_count_bar.png: A grouped bar chart showing the counts of total articles and words in each category for each region of the world. 
6. 06_angry_prop_bar.png: A bar chart showing the proportion of spontaneous/angry words per article for each region. 
7. 07_joy_prop_bar.png: A bar chart showing the proportion of organized/joyful words per article for each region. 
8. 08_prop_bar.png: A grouped bar chart showing both the proportion of spontaneous/angry and organized/joyful words per article in each region. 

## More Information

For more information please contact alia_braley@berkeley.edu