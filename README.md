# Microsoft Studio

# Movie Analysis

##### David Adeola

### Summary

Microsoft aims to enter the original video content market by establishing a new movie studio
and needs to determine which film genres are currently most successful at the box office. Our
analysis utilized three datasets encompassing ratings and votes, movie details, and box office
gross revenues. After data cleaning, preparation, and exploratory data analysis, we identified
that the genres Adventure, Animation, and Comedy have been the most successful in both
domestic and foreign markets over the last five years. Additional promising genres include
Action, Adventure, Sci-Fi, Action, Adventure, Fantasy, Action, Adventure, Comedy, and Action,
Adventure, Thriller, which also demonstrate robust financial success and popularity.

### Summary

Based on these findings, it is recommended that Microsoft's new movie studio
primarily focus on producing Adventure films, as they are the most successful
genre. Additionally, leveraging combinations such as Adventure, Animation,
Comedy and Action, Adventure, Sci-Fi can capitalize on strong audience interest
and substantial box office revenues. This strategy aligns with current market
trends and audience preferences, positioning the studio for success in the
competitive movie industry.

### Outline

#### ● Business Problem

#### ● Data

#### ● Methods

#### ● Results

#### ● Conclusions

### Business Problem

Microsoft sees all the big companies creating original video content and they
want to get in on the fun. They have decided to create a new movie studio, but
they don’t know anything about creating movies. I am charged with exploring
what types of films are currently doing the best at the box office. I have translated
those findings into actionable insights that the head of Microsoft's new movie
studio can use to help decide what type of films to create.

### Data

Dataset 1: Ratings and Votes

Has over 73,000 entries and 3 columns (tconst, averagerating, numvotes). This
dataset provides insights into the popularity and reception of movies, which can
be useful to understand which genres have high average ratings and vote counts,
indicating audience preference.

### Data

Dataset 2: Movie Details

Has over 146,000 entries and 6 columns (tconst, primary_title, original_title,
start_year, runtime_minutes, genres). This dataset provides detailed information
about each movie, including its title, release year, runtime, and genre. It is crucial
for understanding the distribution of movies across different genres and years, as
well as their duration.

### Data

Dataset 3: Box Office Gross

Has over 3,300 entries and 6 columns (studio, title, domestic_gross,
foreign_gross, year). This dataset provides financial performance data for movies,
including domestic and foreign gross revenues. It is essential for understanding
the economic success of different genres and how they perform in different
markets.

### Methods

Data preparation

1. Merging Datasets
   After analysing the data, basic and ratings have a 1:1 mapping compatibility
   as they share a common column tconst. I merged the two datasets by adding
   a reference 'tconst' which derives from basics if basics 'primary_title'
   matches movie_gross 'title'.

### Methods

2. Cleaning Data

I dropped unnecessary columns primary_title, original title as they were
duplicates of title. I also dropped studio as it was not relevant to my analysis. I
converted domestic gross, foreign gross to numerals and removed null values.

### Methods

Data Modeling

- I created a new dataframe of movies grouped by genres to analyze the
  distribution of different genres
- I plotted the genres by foreign gross, domestic gross and ratings to compare
  the performance of different genres
- Aggregated the movies by the top grossing genres and years. I narrowed it
  down to the most recent 5 years to gain the trending genres.

### Results

- 2 of the above graphs, Domestic Gross Sales, Foreign Gross Sales clearly
  show that Adventure, Action and Sci-Fi combination are most successful in
  Domestic and Foreign Gross Sales. It’s clear also to see that the adventure
  genre is popular across the board especially when elements of animation,
  action and or comedy are also included.
- It also shows that the Adventure, Animation, Comedy has been the most
  grossing combination in recent years.
- The ratings graph also supports that out of the top rated movies, Animation,
  Adventure and Comedy was among the top rated

### Conclusions

My recommendation for which type of Movie to produce would be
Adventure, Animation, Comedy as it is the most successful genre in both domestic
and foreign markets in the last 5 years.

Additionally, I also would recommend these based off their recent performances:

1. Action, Adventure, Sci-Fi,
2. Action,Adventure, Fantasy
3. Action,Adventure, Comedy or Action, Adventure, Thriller

Conclusively, I would recommend making Adventure films which are the most
successful

### Repository Structure

├── data
├── images
├── README.md
├── DS Project Presentation-David Adeola.pdf
└── dsc_phase1_project.ipynb
