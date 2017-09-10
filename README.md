The get_home_data file scrapes Portland homes sold between 7/16 and 7/17 from the Portland Maps API. It then scrapes Zillow metadata and Redfin images on those houses.

clean_home_data cleans up the scraped data.

analze_data creates a word vectorization of the realtor description and performs NLP sentiment analysis on it. It also uses VGG16 to get features from the home pictures. It combines the Zillow metadata and this other info into a matrix and then uses Gradient Boosting to predict home prices.

predict_home_prices explores some of the predictions in the test set.
