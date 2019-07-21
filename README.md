## Predicting Lifetime Gross of Documentaries 

Documentaries are the least profitable genre in movies. It is a difficult decision for a lot of really talented filmmakers to go into documentaries. My goal of this project is to understand what variables make a documentary profitable, based on opening gross, ranking, date and name of the studio that produced the movie. 

### Methodology:

1. Scraped data using Beautiful Soup from Box Office Mojo
2. Cleaning data and feature engineering
3. Build the linear regression model
4. Build the RidgeCV model 
5. Build the LassoCV model 

### Data source: 

Ranking of documentaries from 1982 to present - https://www.boxofficemojo.com/genres/chart/?id=documentary.htm

### Target:

- ***MVP***: lifetime gross of movies 
- ***Goal***: Understand the relationship and effects of given features on lifetime gross

### Features:

- Title
- Studio
- Lifetime Gross
- Total theaters showing 
- Opening gross 
- Total theater for opening 
- Year
- Month
- Date 

### Things to consider: 

- In order to use the studio column for my data frame, I will create 29 dummy variable with studios that produced more than 14 documentaries.  
- I will also divide the date by month, year and day. 
