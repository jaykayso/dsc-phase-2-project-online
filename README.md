# King County Housing: Project Two

[Slides and Presentation Folder](https://drive.google.com/drive/u/0/folders/1byjfYdPig3NlDlYQ2rPEEAED-0_ZPD7S)

### Strategic Approach

For this project, I have been tasked with finding the strongest indicators of sale price in the King County Dataset using linear regression techniques that I completed in Module 2 from the Flatiron Data Science Full Time Course.

I've defined my stakeholders as construction developers or real estate developers who are interesting in profiting from building property in the King County area. Information provided online at kingcounty.gov disclose that from 2010 to 2018 the population rose by roughly 400,000 people. Considering that this isn't a high growth rate, this may result in the inability to quickly sell properties which can be a hindrance to developers. Due to this inconvenience, developers would most likely be interested in:

Long term investment of building property and renting it out.
Long term investment of building commercial strip centers and renting them out.

### The Data

The data provided for this project was the King County Dataset. Additionally I pulled average income by zipcode from https://www.incomebyzipcode.com


### Exploratory Questions

[Question One Notebook Link](https://github.com/jaykayso/dsc-phase-1-project-online/blob/master/Question%201.ipynb)
<details><summary style="font-size: 24px">
Question 1: Which genres or themes get the highest ratings?

Data Used: 
    - imdb.title.ratings.csv
    - imdb.title.basics.csv
    
In order to properly calculate the rating average of each genre, I had to split the clusters of the genres so that each cell had one genre with one rating. Then, I was able to calculate the mean with the genres grouped. In conclusion, since Adult and Horror movies average the lowest in terms of rating, I would advise Microsoft agaist creating those movies. 
    
[Question Two Notebook Link](https://github.com/jaykayso/dsc-phase-1-project-online/blob/master/Question%202%20.ipynb)
<details><summary style="font-size: 24px">
Question 2: Does release date impact profit?

Data Used: 
    - tn.movie_budgets.csv
 
I calculated profit by subtracting production budget from the worldwide gross revenue. Then, I calculated profit margin by dividing the profit by the production budget. I grouped this profit margin in terms of weeks of the year and also days of the week to determine if a particular time of release day was more profitable. I quickly found out that sorting by day was mute since the vast majority of movies are released on Friday. Additionally, the highest weeks of movie releases were at the end of the year. The conclusion I drew here was that the movie industry is aware that demand for movies peaks at the end of the week and year. For Microsoft to be successful in the movie space, I would encourage them to take advantage of the peak demand times as well. 
    
[Question Three Notebook Link](https://github.com/jaykayso/dsc-phase-1-project-online/blob/master/Question%203.ipynb)
<details><summary style="font-size: 24px">
Question 3: Can we find writers that show a track record of writing well-rated movies?

Data Used: 
    - imdb.title.principals.csv
    - imdb.title.crew.csv
    - imdb.name.basics.csv
    - imdb.title.ratings.csv
    - imdb.title.basics.csv
    - imdb.title.akas.csv
    
Within the data, the tconst values represent the unique movie titles while the nconst values represent the unique crew names. I separated the clusteers of nconst values and set each to a unique tconst value. I restricted the data to only feature writers. Afterwards, I was able to join that dataframe with movie ratings and create a column that included the count of movies that a particular crew member (nconst) had done. I further restricted the dataframe to only include writers who had written over 5 movies. This made it possible to group by the nconst values (unique crew members) and determine what the average was for each individual writer. I attached the crew names to the short list of qualified writers. In conclusion, I would recommend that Microsoft Studios hire a writer with a track record of successful, highly rated, movies.
    
[Question Four Notebook Link](https://github.com/jaykayso/dsc-phase-1-project-online/blob/master/Question%204.ipynb)
<details><summary style="font-size: 24px">
Question 4: Can we find directors with a track record of directing well-rated movies?

    
 Data Used: 
    - imdb.title.principals.csv
    - imdb.title.crew.csv
    - imdb.name.basics.csv
    - imdb.title.ratings.csv
    - imdb.title.basics.csv
    - imdb.title.akas.csv
    
    
Within the data, the tconst values represent the unique movie titles while the nconst values represent the unique crew names. I separated the clusteers of nconst values and set each to a unique tconst value. I restricted the data to only feature writers. Afterwards, I was able to join that dataframe with movie ratings and create a column that included the count of movies that a particular crew member (nconst) had done. I further restricted the dataframe to only include directors who had directed over 5 movies. This made it possible to group by the nconst values (unique crew members) and determine what the average was for each individual director. I attached the crew names to the short list of qualified directors. In conclusion, I would recommend that Microsoft Studios hire a director with a track record of successful, highly rated, movies.  
    
    
# Wrap Up
    
Microsoft should release a movie on a Friday at the end of the year with a skilled director and writer, and they should avoid the genres of horror and adult. 
    
    
# Future Work
    
I recommend that we further investigate the connection to qualified crew members and movie success. Additionally, it would be interesting to look at a dataset on movie sales and demand on movies year round. 
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    