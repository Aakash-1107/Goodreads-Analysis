#  Goodreads Data Analysis

##  Project Overview
This project analyzes personal Goodreads reading data to uncover patterns in reading habits, rating behavior, and author preferences over time.

The goal of this project is to apply data analysis techniques using Python and visualize insights in a clear and meaningful way.

🇩🇪 German version available here: [README_DE.md](README_DE.md)

--------------------------------

##  Data Cleaning & Preparation
- Converted date columns into proper datetime format
- Extracted "Year" and "Month" from reading dates
- Handled missing values (e.g., Publisher → marked as "Self Published")
- Filtered data for focused analysis (e.g., books read in 2025)

--------------------------------

##  Key Analyses

###  Reading Trends Over Time
- Analyzed number of books read per year
- Identified 2025 as the most active reading year

###  Monthly Reading Patterns (2025)
- Visualized how reading activity varied across months
- Observed peaks and drops in reading behavior

###  Rating Analysis
- Compared personal ratings with average Goodreads ratings
- Identified alignment with general audience preferences

###  Author Insights
- Identified most frequently read authors
- Highlighted reading preferences

###  Publisher Analysis
- Investigated missing publisher data
- Classified unknown entries as "Self Published"

----------------------------------

## Sample Visualizations

###  Books Read per Year
![Books per Year](Charts/books_per_year.png)

###  Books Read per Month in 2025
![Books per Month](Charts/Books_per_month_2025.png)

###  Publisher Distribution
![Rating Comparison](Charts/Publisher_Distribution.png)

###  Rating vs Average Rating
![ View Interactive Version](Charts/Rating_vs_Avg.html)

###  Top Authors
![Top Authors](Charts/Top_Authors_Distribution.png)

----------------------------------

##  Key Insights
- Reading activity significantly increased in 2025
- Reading habits vary across months, with noticeable peaks
- Personal ratings generally align with average ratings
- A portion of books are self-published
- Certain authors are read more frequently, indicating preference patterns

-----------------------------------

##  Tools & Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Plotly

-----------------------------------

##  Future Improvements
- Genre-based analysis
- Recommendation system
- Deeper statistical insights

-----------------------------------


##  Conclusion
This project demonstrates practical data analysis skills including data cleaning, visualization, and insight generation. It highlights how personal data can be used to uncover meaningful behavioral patterns.
