# Statistical analysis of Cars93 dataset in R

(Full report in pdf is located in FuelEconomy  directory)

## Introduction

In this report we will analyze fuel economy of cars in highways with three types of drive-train, namely rear,
front and four wheels drive-train denoted as 4WD. Then we will compare prices of cars according to its origin.
And finally we will look at relation between airbags type and origin of cars. For all three performed analyses
we have used Cars93 dataset.

### Highlights
![drive-train](https://github.com/Many98/Cars93-analyses/assets/65658910/087f96be-cd60-45a2-a707-419f99dd62fa)
![normal_qq](https://github.com/Many98/Cars93-analyses/assets/65658910/9a315d3e-bfd4-47d5-869d-3c86727d8362)
![price_origin](https://github.com/Many98/Cars93-analyses/assets/65658910/d0cd78e2-cbc5-4719-9a5c-5b79b6dce56e)
![qq_2](https://github.com/Many98/Cars93-analyses/assets/65658910/08a31d3e-beda-4f9a-bfe4-35472f63029d)



### Conclusions

According to performed Welch’s ANOVA we can conclude that highway MPG significantly differs among
groups of cars with three types of drive-train with p-value of 0.001. Games-Howell’s test then showed
significant difference in highway MPG only between groups Rear and Front with p-value almost equal to
zero. Similar finding was given by non-parametric Kruskal-Wallis test with p-value of 0.002. Dunn’s test
then revealed that there is also significant difference between groups Front and 4WD with p-value 0.012 in
addition to Games-Howell’s test. As the normality requirement was violated we consider Kruskal-Wallis and
Dunn’s test more trustworthy. Finally we can conclude that cars with front drive-train have higher mean
MPG or in other words lower fuel economy in highways in comparison to cars with rear and 4WD drive-train
and therefore we can say that cars with front drive-train are more economical in highways.

Analysis of prices of cars according to their origin was performed by test of means of prices with asymptotic
test and test of distributions with Kolmogorov-Smirnov test. Both tests turned out to be non-significant with
p-values of 0.340 for asymptotic test of means and 0.517 for Kolmogorov-Smirnov test. As we failed to reject
both of this hypotheses we can only conclude that our data does contain no evidence to say whether prices of
cars are same or not according to their origin. Finally, analysis of homogeneity of distribution of airbags
according to origin of cars was performed using chi squared test which has given also non-significant results
with p-value of 0.79 and we therefore fail to reject hypothesis about homogeneity of distribution of airbags on
significance level of 0.05.
