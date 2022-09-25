# Tarasova HW1 Kinopoisk

Here we tested  Mann-Whitney U test and Bootstrap.

 Mann-Whitney U test pecularities:
- we can use it without data normalization
- and when sample size is small

As for Bootstrap, this technique allows to estimate of the sampling distribution of almost any statistic using random sampling methods

This is critical for us, because dataset sample is mall (only 250 records).
Lets assign our hypothesis:

 H0 - there is no statistical difference between rating_new and rating_old
 Ha - the difference between rating_new and rating_old exists
 
 Conclusion: both for Mann-Whitney U test and Bootstrap we did not get any statistical difference between old and new ratings, when applied to the whole dataset. Therefore, we tried to group it by Country and genre and there is were differences start to show. We choose USA action movies.
 
 Mann-Whitney U test pvvalue was less then 0.05, which proves, that there is statistical difference. Unfortunately, it was not supported by bootstrap, because our dataset is small (only 33 rows), therefore, when we resample it, using bootstrap, we did not get that difference between two groups is relevant. Old rating does not differ from new rating
 
