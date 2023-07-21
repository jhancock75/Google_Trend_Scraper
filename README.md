# Google Trend Scraper
Created a script in Python that utilizes the PyTrends package to scrape up to 5 keywords at time, which is then stored in a time series 

Visualizations are then created for both the raw time series data and the data on a 7-day moving average.

Then 3 final dataframes are created each for geographic breakdowns, 1 for state, 1 for DMA, and 1 for city.

**Script can be limited by Google's rate limit, although v4.9.2 of PyTrends should have solved the majority of issues, as well as changing line 88 of "request.py" to a .post() method instead of a .get() method and adding 3 retries (with 3 second intervals) to the scraper script itself.
