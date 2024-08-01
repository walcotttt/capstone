# TKH Capstone Project 2024

The following is a statistical analysis of the 2023-2024 Boston Celtics rosters' gamelog statistics, including  3-Point Field Goal %, Total Rebounds, and +/-. I began by web scraping relevant data. Then I completed exploratory data analysis which informed the key summary statistics I used in my Tableau dashboard. 

## Web Scraping: Data Collection

All of the data used in this project comes from [Basketball Reference](https://www.basketball-reference.com/), an open source website and "invaluable resource for writers, number-crunchers and fans" (Robert Bradley, president of the Association for Professional Basketball Research and author of The Compendium of Professional Basketball).

Once I compiled every member of the 2023-2024 Boston Celtic's roster's gamelogs into a single dataframe, I output the result into a .csv file which I then used as the foundation of my analysis.

## Exploratory Data Analysis

Since the first three columns of the dataframe ('Unnamed: 0', 'Rk', 'G') were all indexes of sorts, I opted to drop them. In the process of cleaning the data I realized that column titles repeated throughout various rows on the df. The columns affected included: Date, Age, Tm, Opp, GS, MP, FG, FGA, FG%, 3P, 3PA, 3P%, FT, FTA, FT%, ORB, DRB, TRB, AST, STL, BLK, TOV, PF, PTS, GmSc, and +/-.