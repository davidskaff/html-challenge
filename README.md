# Mars Data Scraping and Analysis Project

This project involves scraping and analyzing data from Mars. Here's a brief summary of the project:

## Part 1: Scraping Titles and Preview Text from Mars News

The project begins with the creation of the Jupyter Notebook `part_1_mars_news.ipynb`. Automated browsing was used to visit the Mars news site, and the page was inspected to identify the elements to scrape.

A Beautiful Soup object was created and used to extract text elements from the website. The titles and preview text of the news articles were extracted and each title-and-preview pair was stored in a Python dictionary with two keys: `title` and `preview`.

All the dictionaries were stored in a Python list and displayed in the notebook. Optionally, the scraped data was exported to a JSON file for easier data sharing.

## Part 2: Scraping and Analyzing Mars Weather Data

The next step involved creating the Jupyter Notebook `part_2_mars_weather.ipynb`. Automated browsing was used to visit the Mars Temperature Data Site, and the page was inspected to identify the elements to scrape.

Another Beautiful Soup object was created and used to scrape the data in the HTML table. The scraped data was assembled into a Pandas DataFrame. The columns correspond to the headings on the website:

- `id`: the identification number of a single transmission from the Curiosity rover
- `terrestrial_date`: the date on Earth
- `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
- `ls`: the solar longitude
- `month`: the Martian month
- `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
- `pressure`: The atmospheric pressure at Curiosity’s location

The data types associated with each column were examined and cast to the appropriate datetime, int, or float data types if necessary.

The dataset was analyzed using Pandas functions to answer several questions about Mars, such as the number of months on Mars, the coldest and warmest months on Mars, and the months with the lowest and highest atmospheric pressure. The results were plotted as bar charts.

Lastly, the number of terrestrial (Earth) days in a Martian year was estimated by considering how many days elapse on Earth in the time that Mars circles the Sun once. The result was visually estimated by plotting the daily minimum temperature.
