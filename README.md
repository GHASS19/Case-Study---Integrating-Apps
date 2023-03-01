# Integrating Apps Case Study

![image](https://user-images.githubusercontent.com/86930309/222280033-f03e2a62-1024-4319-a972-ac927201e676.png)

# 1. Sourcing and loading

- Load the two datasets
- Pick the columns that we are going to work with:

1. Google: 

a. Category (Do we need this?)

b. Rating

c. Reviews

d. Price (maybe)

2. Apple:

a. prime_genre (Do we need this?)

b. user_rating

c. rating_count_tot

d. price (maybe)

- Subsetting the data on this basis

# 2. Cleaning, transforming and visualizing

- Check the data types and fix them
- Add a platform column to both the Apple and the Google dataframes
- Changing the column names to prepare for a join
- Join the two data sets
- Eliminate the NaN values
- Filter only those apps that have been reviewed at least once
- Summarize the data visually and analytically (by the column platform)

# 3. Modelling

- Hypothesis formulation
- Getting the distribution of the data
- Permutation test

# 4. Evaluating and concluding

- What is our conclusion?
- What is our decision?
- Other models we could have used.
