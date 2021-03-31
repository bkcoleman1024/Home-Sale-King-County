# Home-Sale-King-County

# Overview
There are many factors that can influence the price of a home. Real estate professionals may have an idea of the best factors but are these current trends or are they out of date?
Based on recent home sales I will examine the features of these homes to see if there are trends that effect the sales price.

# Business Problem
There are many factors that can contribute to a sales price.  This project is looking into potential home improvement projects.  

# Data Understanding
The data has been collected for home sales in King County, WA.  The data contains all of the real property sales from 2019.  The data contains information from commercial and residential properties.  Depending on the features that I was evaluating, the sample sizes ranged from 50,000-70,000.

# Methods
The data was examined and cleaned.  The focus of this project was on residential properties.  Anything other than houses and condos were removed.  The sales price for properties ranged from zero to over $15 million.  Although it is still low, all sales prices less than $25,000 were removed.

A linear regression model was used to examine the information.  Since there were several features that were provided by the data, a correlation matrix was produced to have a better opportunity to find features that correlate with the sales price.
After selecting several features, I used a pairplot to examine this features more.  

The final model had an R-squared of .353.  This model was used to examine specific categories.  I looked into the heat source and an enclosed porch. 

For the heat source I looked at electric and electric plus solar.  The R-squared is .432.  The heat source coefficient is 44,270.  The sales price on average could increase by this amount by adding a solar feature.  The rainbow p-value is rather low.  The current model does violate the linearity assumption.  Given the low JB probability the current model also violates the normality assumption.

I also looked at adding an enclosed porch.  The R-squared is .397.  The porch coefficient is 73,880.  The sales price on average could increase by this amount by adding an enclosed porch.  The rainbow p-value is also low.  The current model does violate the linearity assumption.

# Results

I would recommend adding a solar feature or an enclosed porch.  There is the potential for a significant increase to the sales price.  

- Adding a solar feature increased the sales price on average by 44,270.
- Adding an enclosed porch increased the sales price on average by 73,880.

# Conclusions

While these models did produced possible recommendations for home imporovement projects, there is still the need for additional research.  

For this project I only considered one heat source, electric.  Would the results be similar if the heat source was gas or oil?

Further analysis also needs to be done regarding the porch.  I looked at enclosing a porch.  Although it would not apply to all residences, would simply adding a porch increase the potential sales price of a home?
