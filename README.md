# REG-2022-03-18
What Impact Does Possession Rate Have on Success

By: Burak Basogul

Abstract

The client who is a director of planning in a first tier soccer league (Super Lig) in Turkey, is in preparation for implementing a new five year term project
and interested in identifying statistics that the most successful teams exhibit in first tier soccer leagues with a focus on determining the impact of 
possession rate on success

Design
League tables with available possession rate stats for Super Lig and top 8 European leagues are web scraped using Beautiful Soup and manipulated in Pandas and combined into one single data set. A baseline modeling is conducted on available data from Super Lig but the limited available did not allow for production of a reliable model just for Super Lig. However, selection of features for the baseline is validated during modeling of the  top 8 European (UEFA)leagues. 
For the main modeling of the UEFA Leagues, the available data is from  2015 thru 2022 consisting of 1,088 rows and 14 features. Target label is set as Possession Rate and data is split into training, validation and test sets (60, 20, 20). Feature selection is based upon eliminating col-linearity using stats-models package. Training and validation test scores are also obtained using scikit-learn package as a back check and proved to be within 0.02 points from each other. Final model is selected to be Lasso Regression albeit with modest score improvement over Simple Regression with a final R^2 score of 0.601.


Data

League Tables as of end of season for each 8 league and Super Lig joined with Squad Standard Stats are web scraped from https://fbref.com/


Algorithms & Tools

1. Base code extracting data via HTML links by Metis in Beautiful Soup Exercises was used to selectively take in and parse data using beautiful soup.

2. Pandas to manipulate and join tables.

3. Stats-models and scikit-learn packages for Linear Regression modeling.

4. Seaborn for generating visuals



Communication
•	Project presentation slides (Info on slides reflects scores achieved during initial iteration of the models which did not included 2022 data)
