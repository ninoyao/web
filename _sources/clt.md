# What Central Limit Theorem does?

The Central Limit Theorem is often referred to as the “cornerstone of statistics”. It is the fundamental concept you have to understand before performing any data analysis.

## Why can we estimate the avg height among students in a university by only sampling (Obtaining data) a part of them? — Central Limit Theorem

## Why can we estimate the avg family income of America without asking every family in the United States? — Central Limit Theorem

# How does Central Limit Theorem help us?

As collecting data of every student in a university is time-consuming and collecting the annual income of every American family is impossible, we need a reliable way to “estimate” the true value.

The Central Limit Theorem solves this problem.

It says that the means drawn from multiple samples will resemble the familiar bell-shaped normal curve, even if the source population is not normally distributed.

## A normal distribution

<Practical statistics for data science> The first plot.

- We randomly pick 1000 samples from the original dataset. From the histogram, we can find that its distribution is not “bell-curved”, which means, it is not normally distributed.

The second plot.

- We randomly pick 5 samples from the dataset at once and calculate their mean, then repeat this process for 1000 times so that we have 1000 means of 5 random samples from the dataset. From the histogram, we can find that the second plot is more bell-shaped.

The third plot.

- We randomly pick 20 samples from the dataset at once and calculate their mean, then repeat this process for 1000 times so that we have 1000 means of 20 random samples from the dataset. From the histogram, we can find that the third plot is less spread than the second one.

### Why is it?

- Back to the original dataset. The probability of picking a value larger than 150,000 from this dataset is 2.458%.

- What’s is the probability of having a mean of 4 samples larger than 150,000? You will need to constantly pick 4 values around 150,000. Thus the probability is less than 2.458%.

- When we repeat our sampling and calculate their mean, we will have a more “bell-curved” plot. As the probability of having an extreme value decreased and the probability of having a “mean close” value increased.

- This also leads to another conclusion. The bigger the sample size for calculating the mean is, the smaller the distribution spread is.

## Other voice

- Some people hold the idea that, Data scientists should be aware of this role, but, since formal hypothesis tests and confidence intervals play a small role in data science, and the bootstrap is available in any case, the central limit theorem is not so central in the practice of data science.

Is that correct? Tomorrow I will introduce the bootstrap and discuss more about it.
