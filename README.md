# Google Trend Scraper
Created a script in Python that utilizes the PyTrends package to scrape search frequency data for up to 5 keywords at time. 

The script is broken down into 3 parts:
1. Keyword search interest aggregated at the country level (US) over 1 time period
2. Keyword search interest aggregated at the state level (US) over 1 time period
3. Keyword search interest between 2 time periods by state (US)

The 1st section aggregated at the country level has a time series plotted for the search interest with each keyword being a single line.

All 3 of the sections have a corresponding descriptive statistics table that is also plotted as a bar chart.

At the very end, you are able to export the data from each section (including descriptive statistics) as a .csv file.

**Script can be limited by Google's rate limit, although v4.9.2 of PyTrends should have solved the majority of issues, as well as changing line 88 of "request.py" to a .post() method instead of a .get() method and adding 3 retries (with 3 second intervals) to the scraper script itself.
