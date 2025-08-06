## **Movie Industry Analysis: Data-Driven Insights for New Movie Production**

This project explores movie data to identify the key factors that contribute to box office success. Using data from Box Office Mojo, The Numbers and IMDb, the analysis provides actionable insights that a new movie studio can use to select the best film types to produce. The focus is on uncovering patterns in genre performance, production budgeting and release timing to guide informed and data driven film production decisions.


## 1. Business Understanding

**Business Objective**:
To guide film production decisions using data that reveals trends associated with box office revenue.

**Stakeholder**:
Head of the new movie studio responsible for deciding which film projects to pursue.

**Business Questions**:

1. Which movie genres have the highest average box office revenue?
2. How does production budget influence gross earnings?
3. Which release months are associated with higher box office performance?


## 2. Data Understanding

**Data Sources Used**:
Out of all provided datasets, three were selected for their relevance:

* **Box Office Mojo** (`bom.movie_gross.csv.gz`) – Domestic box office revenue
* **IMDb** (`im.db.zip`) – Movie titles, genres, ratings, release years
* **The Numbers** (`tn.movie_budgets.csv.gz`) – Budgets and worldwide gross

**Exploratory Tasks**:

* Inspected data formats (CSV, SQLite)
* Identified missing or inconsistent values
* Selected only datasets relevant to the defined business questions

**Datasets Not Used**:

* TMDb and Rotten Tomatoes were excluded due to redundancy or irrelevance to stakeholder objectives


## 3. Data Preparation

**Cleaning and Transformation Steps**:

- Removed irrelevant columns
- Renamed columns for clarity
- Converted data types
- Dropped missing values
- Merged datasets using movie titles and release years

**Final Output**:
A cleaned and merged dataset (`final_merged_df`) containing relevant features for data analysis.


## 4. Modeling

This project focused on Exploratory Data Analysis (EDA). No machine learning models were developed. Instead, the analysis relied on grouped aggregations, correlation analysis and time based trend analysis.


## 5. Evaluation

Each business question was evaluated using visualizations and statistical summaries derived from the cleaned dataset.

- For the first question, a bar chart of average worldwide gross by genre showed that Action, Adventure and Animation genres consistently generated the highest returns. Action films, in particular, averaged over \$250 million globally.

- For the second question, a scatter plot was used to compare production budget against worldwide gross. While the overall correlation was positive, outliers revealed that only certain high budget films delivered exceptional returns. Films with budgets between \$50M to \$100M showed a balanced risk return profile.

- For the third question, a bar chart of average worldwide gross by release month revealed that May, June, November and December were the strongest months. Films released during these months grossed up to 35% more on average than those released in low performing months like January or September.

These insights directly support the business objective by identifying patterns in genre selection, budget allocation and release timing that are most strongly associated with box office success.


## 6. Deployment

The findings were communicated through:

- A Jupyter Notebook (`movies.ipynb`) containing the full analysis

- A Tableau Dashboard: [Movie Industry Analysis][https://public.tableau.com/app/profile/jessica.gichimu/viz/MovieIndustryAnalysis_17544451810610/MovieIndustryAnalysis?publish=yes] with four stakeholder focused visuals

- A PDF presentation

## 7. How to Run or Reproduce

**Environment Setup**:

- Python

- Jupyter Notebook

- Required libraries: `pandas`, `sqlite3`, `matplotlib`, `seaborn`

**Run Instructions**:

1. Clone the repository

2. Open `movies.ipynb` in Jupyter Notebook

3. Run cells sequentially to reproduce the full analysis and visual outputs


## 8. Dashboard Summary

The Tableau dashboard includes four visualizations aligned with the business questions:

1. Top 10 Movie Genres by Average Gross – A horizontal bar chart displaying the average worldwide gross for the top performing genres.

2. Relationship Between Production Budget and Gross Revenue – A scatter plot with a regression line highlighting the positive correlation between budget and box office performance.

3. Box Office Revenue by Release Month – A bar chart showing how total gross revenue varies by release month, revealing strategic timing for film launches.

4. High Budget Films by Genre – A bar chart showing which genres are most frequently associated with high production budgets showing where studios are most willing to invest.

These visuals help stakeholders make informed production and scheduling decisions.


## 9. Key Insights

- Top performing genres. Action, Adventure, and Animation led in average worldwide gross, with Action films grossing over \$250M on average.

- Budget performance relationship. High budget films tend to earn more but mid tier budgets of about \$50M to \$100M offer a balanced approach with lower risk.

- Release timing. May and June, November and December are the most strategic months yielding up to 35% higher average revenue.


## 10. Recommendations

1. Focus on high return genres. Prioritize Action, Adventure films which have stronger returns.

2. Strategically allocate budgets. Use mid tier budgets for testing market response and reserve large budgets for franchises.

3. Diversify portfolio. Include lower budget films to explore different genres while minimizing risk.


## 11. Future Work

- Explore audience ratings and sentiment from Rotten Tomatoes


## 12. Contributor

This project was completed by Jessica Gichimu

**Data Providers**:

- IMDb
- Box Office Mojo
- The Numbers


## 13. Conclusion

The project delivered actionable and evidence based recommendations for film production planning. It shows the importance of data analysis in solving real world business problems and supports decision making.
