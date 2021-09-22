# Proposal

## Question
Stanley of Fred and Mabel Yarns wants to know how much to price his knitting patterns for sweaters. He doesn't want to charge too much, but he wants his hard work to pay off! I will use data from Ravelry.com to find a comparable price for his patterns, given the various features of the sweater in the pattern. 

## Tools
I will use BeautifulSoup and Selenium to scrape data from Ravelry.com's patterns, Pandas to clean the data, linear regression to model the data, and matplotlib and seaborn to display the data. 

## Samples
An individual sample is a single pattern page from Ravelry.com. On the page, there are various pieces of information about the pattern including how many projects have been started from it; which craft (knitting, crochet, etc.); recommended yarn; at least one photo of a finished project; and other data. 

The features I will use for the regression will be 7 of the 11 categories on each project page ("craft", "yarn weight", "gauge", "needle size", "yardage", "sizes available", "languages"); number of projects; and the tags, which include information about various skills used in making the sweater. The price of the pattern is the target.  

## MVP 
MVP will be a linear regression of number of projects vs. price. This will give an average price of patterns given the number of people who have made the pattern.
