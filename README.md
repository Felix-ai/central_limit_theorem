## CENTRAL LIMIT THEOREM

### Introduction

The central limit theorem states that if you have a population with mean μ and standard deviation σ and take sufficiently large random samples from the population with replacementtext annotation indicator, then the distribution of the sample means will be approximately normally distributed. This will hold true regardless of whether the source population is normal or skewed, provided the sample size is sufficiently large (usually n > 30). If the population is normal, then the theorem holds true even for samples smaller than 30. In fact, this also holds true even if the population is binomial, provided that min(np, n(1-p))> 5, where n is the sample size and p is the probability of success in the population. This means that we can use the normal probability model to quantify uncertainty when making inferences about a population mean based on the sample mean.


### Central Limit Theorem with a Normal Population

The figure below illustrates a normally distributed characteristic, X, in a population in which the population mean is 75 with a standard deviation of 8.

![CLT_with_normal_population](images/norm_population.png)

If we take simple random samples (with replacement)text annotation indicator of size n=10 from the population and compute the mean for each of the samples, the distribution of sample means should be approximately normal according to the Central Limit Theorem. Note that the sample size (n=10) is less than 30, but the source population is normally distributed, so this is not a problem. Note that the horizontal axis is different from the previous illustration, and that the range is narrower.

![CLT_with_normal_population_sample_means](images/norm_population_sample_means.png)


### Central Limit Theorem with a Dichotomous Outcome

Suppose we measure a characteristic, X, in a population and that this characteristic is dichotomous (e.g., success of a medical procedure: yes or no) with 30% of the population classified as a success (i.e., p=0.30).

![CLT_with_dichotomous_outcome](images/dichotomous_outcome.png)

The distribution of sample means based on samples of size n=20 is shown below.

![CLT_with_dichotomous_outcome_sample_means](images/dichotomous_outcome_sample_means.png)


### Central Limit Theorem with a Skewed Distribution

The Poisson distribution is a probability model that is useful for modeling discrete variables such as the number of events occurring during a given time interval. For example, suppose you typically receive about 4 spam emails per day, but the number varies from day to day. Today you happened to receive 5 spam emails. What is the probability of that happening, given that the typical rate is 4 per day?

![CLT_with_poisson_population](images/poisson_population.png)

This population is not normally distributed, but the Central Limit Theorem will apply if n > 30. Also note that the sample standard deviation (also called the "**standard error**") is larger with smaller samples, because it is obtained by dividing the population standard deviation by the square root of the sample size. Another way of thinking about this is that extreme values will have less impact on the sample mean when the sample size is large.

![CLT_with_poisson_population_sample_means](images/poisson_population_sample_means.png)
