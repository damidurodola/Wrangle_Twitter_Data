# Wrangle and Analyze Twitter Data

I wrangled, analyzed and visualized archived tweet relating to WeRateDogs twitter account.

## Introduction
The dataset is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs). WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "[they're good dogs Brent.]"(http://knowyourmeme.com/memes/theyre-good-dogs-brent) WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs [downloaded their Twitter archive](https://support.twitter.com/articles/20170160) and sent it to Udacity via email exclusively for use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

## Project Overview
The following tasks are required to complete this project:
### Gathering Data

Data was gathered from three datasets:
  - Enhanced Twitter Archive: The CSV file is required to be downloaded manually through a link provided by Udacity. The dataset contains 5000+ tweeets which needs to be assessed and cleaned.
  - Additional Data via the Twitter API: Using the tweet IDs from the enhanced twitter archive dataset,additional information such as retweet and favourite count are retrieved and saved in a JSON file. Twitter's API is queried using the Python's Tweepy library and each tweet with it's related information is stored on a line in the JSON file. To query Twitter's API, you need to have a twitter account and [setup a developer's account](https://developer.twitter.com/en/docs/basics/developer-portal/overview).
  - Image Predictions File: This dataset contains image predictions of dogs breed. Each dog image was run through a neural network to generate this information. The dataset is to be downloaded programmatcally using the requests library.

### Assessing Data
After gathering all three pieces of data, assess them visually and programmatically for quality and tidiness issues. Detect and document at least eight (8) quality issues and two (2) tidiness issues in the "Accessing Data" section in the `wrangle_act.ipynb` Jupyter Notebook.

### Cleaning Data
Clean all of the issues documented while assessing. The following steps are required to complete this stage:
  - Before you perform the cleaning, you will make a copy of the original data.
  - During cleaning, use the define-code-test framework and clearly document it.
  - Cleaning includes merging individual pieces of data according to the rules of tidy data. The result should be a high-quality and tidy master pandas DataFrame (or DataFrames, if appropriate).

### Storing Data
Stored the cleaned master DataFrame in a CSV file named `twitter_archive_master.csv`.

### Analyzing and Visualizing Data
Analyze and Visualize data to produce at least three (3) insights and one (1) visualization.

### Reporting Data
Create a 300-600 word written report called `wrangle_report.pdf` or `wrangle_report.html` that briefly describes the wrangling efforts. Also, create a 250-word-minimum written report called `act_report.pdf` or `act_report.html` that communicates all the insights and displays the visualization(s) produced from your wrangled data.
