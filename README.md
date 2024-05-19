# Data Collection - Web Scraping

This challenge consists of two technical products: The first part will scrape titles and preview text from Mars news articles; and on part two, it will scrape and analyze Mars weather data, which exists in a table.

## Part 1: Scrape Titles and Preview Text from Mars News
The Jupyter Notebook used for this part is 'mars_news.ipynb' to be able to scrape titles and preview the text from Mars News folowwing the next steps:

1. Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.

2. Create a Beautiful Soup object and use it to extract text elements from the website.

3. Extract the titles and preview text of the news articles scraped. Store the scraping results in Python data structures as follows:
    - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview.
    - Store all the dictionaries in a Python list.
    - Print the list in the notebook.

## Part 2: Scrape and Analyze Mars Weather Data
Using automated browsing the Jupyter Notebook 'mars_weather.ipynb' will visit the Mars Temperature Data SiteLinks, inspect the page to identify elements to scrape and analyze Mars weather data following the next steps:

1.  Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website:

- id: the identification number of a single transmission from the Curiosity rover
- terrestrial_date: the date on Earth
- sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
- ls: the solar longitude
- month: the Martian month
- min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
- pressure: The atmospheric pressure at Curiosity's location

4. Examine the data types that are currently associated with each column and cast (or convert) the data to the appropriate datetime, int, or float data types.

5. Analyze the dataset by using Pandas functions to answer the following questions:

- How many months exist on Mars?
- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
- What are the coldest and the warmest months on Mars (at the location of Curiosity)?:
    - Find the average minimum daily temperature for all of the months.
    - Plot the results as a bar chart.
- Which months have the lowest and the highest atmospheric pressure on Mars?:
    - Find the average daily atmospheric pressure of all the months.
    - Plot the results as a bar chart.
- About how many terrestrial (Earth) days exist in a Martian year?:
    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimate the result by plotting the daily minimum temperature.

6. Export the DataFrame to a CSV file.