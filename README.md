# tmdb_movies_dataset_python_analysis

Description: This project takes the TMDB Movies dataset of over 10,800 films and turns it into clear insights on what drives box office success. I cleaned the data with Python (pandas and numpy) by removing duplicates and filtering out records where budget or revenue was recorded as 0, which cut the dataset down to about 3,850 reliable movies. I then explored the cleaned data to answer two questions: whether bigger budgets lead to higher revenue, and which genres are the most profitable. The analysis found a positive correlation of about 0.69 between budget and revenue, and showed that Animation, Adventure, Fantasy and Family films earn the highest average profit.

1. Tech Stack

The project was built using the following tools and technologies:

🐍 Python (pandas, numpy): Loaded the raw movie data, checked data types and missing values, removed duplicates, filtered invalid budget and revenue records, and created a new profit metric (revenue minus budget).

📓 Jupyter Notebook: Used to write and document the full wrangling and analysis workflow step by step.

🧹 Reusable Python functions: Built a clean_financials() function for the cleaning steps and a format_plot() function to keep chart titles and labels consistent.

🔀 Pandas string and explode methods: Split multi-genre entries like "Action|Adventure" into separate rows so each genre could be analyzed on its own.

📈 Pandas plotting (Matplotlib): Built histograms for budget and revenue distributions, a scatter plot of budget vs. revenue, and a bar chart of average profit by genre.

📊 Correlation and groupby analysis: Measured the budget-revenue relationship and ranked genres by average profit.

2. Key Insights

Most movies have small budgets and modest revenue, while only a few blockbusters sit at the top end.

Budget and revenue have a correlation of about 0.69, so bigger budgets often mean bigger revenue, but it is not guaranteed.

Animation had the highest average profit (about $180M), followed by Adventure, Fantasy and Family.

Documentary and Foreign films had the lowest average profit.
