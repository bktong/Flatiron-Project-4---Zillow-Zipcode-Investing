
# Module 4 -  Final Project Specifications


### The Project Objective

For this project, you will be acting as a consultant for a fictional real-estate investment firm. The firm has asked you what seems like a simple question:

> what are the top 5 best zipcodes for us to invest in?

This may seem like a simple question at first glance, but there's more than a little ambiguity here that you'll have to think through in order to provide a solid recommendation. Should your recommendation be focused on profit margins only? What about risk? What sort of time horizon are you predicting against?  Your recommendation will need to detail your rationale and answer any sort of lingering questions like these in order to demonstrate how you define "best".

As mentioned previously, the data you'll be working with comes from the [Zillow Research Page](https://www.zillow.com/research/data/). However, there are many options on that page, and making sure you have exactly what you need can be a bit confusing. For simplicity's sake, we have already provided the dataset for you in this repo--you will find it in the file `zillow_data.csv`.

### Project Overview
The project goal is to explore time series modeling and forecasting.  We are wrapping it around a fictional exercise of being a consultant to a client looking to invest.
As we have been given a lot of freedom to define and shape our use-case I have selected the following scenario for this project.

### Files Included

Readme.md                   - this file
LICENSE.md                  - License
zillow_data.csv             - csv with our zillow zipcode data
Mod 4 Project.ipynb         - Jupyter Notebook of our project code
/zillow/zip_MedianRental*   - rental data from zillow's research page.


# Project Summary:
# The Client:   Boutique REIT seeking to invest $1.5-2 mil.
The client is a small partnership-based real estate investment trust with $1.5 to $2 Million on hand that would like to create an exciting portfolio with the goal of attracting additional investors.   They have asked us to help them pare down there initial search.   They are not tied to any area specifically and plan to set up operations in a metro area that makes sense.   

The client's portfolio strategy is to invest in single-family homes and turn those into rental properties.  They are seeking top level guidance using a disciplined data-driven approach to starting their rental portfolio.

# Key Metric:
Return on Investment: We don't have much in terms of cost data to work with so a true ROI calculation doesn't pertain.  We are however, using a proxy calculation for ROI to so we can compare our zip codes on an apples to apples basis.    We will be using the calculation of annual rent collected as a percentage of home price.   The higher the percentage the better for our portfolio.

# Summary:
Zip codes are just a starting point for our firm.   There are plenty of attractive options when we are looking at investment properties as rental units.  With 20+ zipcodes in Houston offering double digit returns.   We provide our client with the following zipcodes as our Top 5, but would have encouraged them to look a properties in almost all of our top 20.

Our Top 5
77073
77338
77396
77373
77083

### Process and Design

This was a very open ended project.  We had to decide on a story to follow and see the analysis through in a way that made sense to our "client."   In the end I tried to show how the design of our question played a major role in how sought the answer it.

Process:

We needed to take a look at the data and understand what kind of question could we answer with it that actually made any sense.   Investment is such a vague term here, but investing in one zip code over another makes zero sense because real estate is about investing in assets not zip codes.

ultimately we decided we needed additional outside data to peg our analysis on, so we we went back to the original source (zillow) to see what they had.   Rental data came up and it was conveniently formatted in a similar manner to the data we were provided.    

Filtering out our data:   It made sense as a preprocessing move to figure out a good way to filter out most of our data.  I used the story of seeking a center of operations to invest in nearby zipcodes, but it could have been as simple as picking a city like Chicago.  We were able to calculate our ROI to drive our decision making to further analyze Houston zip codes.

Forecasting:  We ended up using a SARIMAX model for our time series because our data was very much seasonal.   We learned how to apply different pdq combinations and seek out the optimal one to tell our stories.  In the end we were able to select 5 for further exploration, but obviously did not have the data to drive anything truly resembling an investment decision.

### Findings
time series modeling makes sense on paper, but requires many tiny steps with lots of variables to keep track of.   I really needed to sit down and organize my thoughts about what exactly was needed and how I was going to be able to access that data at the time.    It is definitely worth our time to work alongside in a notebook / or with MANY comments to keep track of where you in case life circumstances breaks your concentration.


End of Mod 4 project
