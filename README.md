# Integrating Apps Case Study

![image](https://user-images.githubusercontent.com/86930309/222280033-f03e2a62-1024-4319-a972-ac927201e676.png)

# Our main objective is to find out if Apple Store apps received better reviews than the Google Play apps?

# 1. Sourcing and loading

- Load the two datasets.

- Pick the columns that we are going to work with:

### Google: 

a. Category (Do we need this?)

b. Rating

c. Reviews

d. Price (maybe)

### Apple:

a. prime_genre (Do we need this?)

b. user_rating

c. rating_count_tot

d. price (maybe)

- Subsetting the data on this basis.

# 2. Cleaning, transforming and visualizing

- Check the data types and fix them. Changed the data type of a few columns.
- Add a platform column to both the Apple and the Google dataframes. Now we can add both dataframes together and compare the reviews.
- Changing the column names to prepare for a join.
- Join the two data sets.
- Eliminate the NaN values.
- Filter only those apps that have been reviewed at least once.
- Summarize the data visually and analytically (by the column platform).
- Apple has a mean user rating of 4.049697.
- Google has a mean user rating of 4.191757.

![image](https://user-images.githubusercontent.com/86930309/222649259-6032c723-5137-4ee8-9d21-16cc14a993f3.png)

The boxplot shows the distribution of the ratings.

# 3. Modelling

- Hypothesis formulation:

null: the observed difference in the mean rating of Apple Store and Google Play apps is due to chance (and thus not due to the platform).

alternative: the observed difference in the average ratings of apple and google users is not due to chance (and is actually due to platform)

The significance level will be 0.05.

- Getting the distribution of the data:

Apple's left skewed ratings distribution
![image](https://user-images.githubusercontent.com/86930309/222650214-381e48ab-0e7e-459c-8c39-76e92fd3dcdb.png)

Google's left skewed rating distribution
![image](https://user-images.githubusercontent.com/86930309/222650358-9dc8ab19-e630-4fb0-becd-476969b5fbfe.png)

- Permutation test

![image](https://user-images.githubusercontent.com/86930309/222651491-363111e8-8d8e-471c-a88c-117054e3eee8.png)

Here we have a pretty normal distribution after simulating 1,000 permutations of the average platforms ratings.

# 4. Evaluating and concluding

- conclusion

Our observed data is statistically significant. The p-value is 0 and we will reject the null.

- Decision

The platform does have an impact on ratings. We will advise our client to integrate only Google Play into their operating system interface.


