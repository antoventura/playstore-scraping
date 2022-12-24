# playstore-scraping

#### Scraping reviews for category in play store using selenium and reviews descriptive statistics for business insight using knime

On play.google.com is not possible to search app for categories (24 Dec 2022), so it is not possible to scrape on the website directly to gather data for a specific category.
The python script on the ipynotebook creates a dataset scraped using Selenium and Beautiful Soup, first gathering data from one of the most reliable websites for app store world charts, APPlyzer 2 and, then, using the id of the app to scrape reviews on play store

For the optimal evaluation of the success and failure parameters of
an application, it was carefully selected to download only 1-star, 3-star, and 5-star ratings.
The created dataframe on 20 Dec 2022 contains 63'144 entries in total, divided into two columns for the rating and its review, with a balanced number of reviews for each rating.

On Knime, instead, all the preprocessing of the data and the Text mining procuedure take place:

The ultimate objective of any text mining process using the “bag-of- words” approach is to convert the text to be analyzed into a data frame that consists of the words used in the text and their frequencies. These are defined by the document term matrix
(DTM) and the term document matrix (TDM); to ensure that the DTM and TDM are cleaned up and represent the core set of relevant words, a set of pre-processing activities needs to be performed on the corpus.

Finally the knime workflow outputs wordclouds, bar charts and pyramid graphs for descriptive statistics purposes
