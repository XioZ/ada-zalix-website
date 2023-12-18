# 3. Ethnic Diversity
<!-- exploratory analysis: ethnic diversity as an interesting factor to set the stage 
    - [x] expect good films to have a higher proportion of films with greater ethnic diversity among cast -->

Hollywood, and many major film studios around the world, have long faced criticism for the lack of racial diversity in its workforce both on and off the screens. In recent decades, there has also been a growing call for greater representation of racial minorities on the silver screen. [Figure 3.1] shows a quick exploratory analysis of the distribution of the number of ethnicities among cast members of each film between 1900 to 2009. As shown in the figure, the curve representing films rated 7 or above is consistently higher than that of films rated below. This suggests that highly rated films generally have more ethnically diverse casts than those lower rated. 

![Figure 3.1: CCDF of Number of Cast Ethnicities in High-Rating vs Lower-Rating Films](./assets/img/3.1.png)

## 3.1 Shifting Demographics: From Diverse Actors Pool To Diverse Cast
<!-- ethnic demographic change among actors (# actor ethnicities) over time AND ethnic diversity change among cast/on-screen (# cast ethnicities) over time 
    - [x] expect upward trends in both => shift in actor ethnic demographics reflected by greater ethnic representation on screen -->

To set the stage, let's first take a look at how the ethnic demographic of actors has evolved globally over time. [Figure 3.2] shows that the 110-year history of film-making has witnessed a booming growth in the ethnic background of actors, with the trend accelarating after 1960s.

This fast diversifying shift in the acting workforce is reflected on the silver screen, through greater, though much more subdued, ethnic representation by the collective featuring of actors from different ethnic background in the same films.

![Figure 3.2: Number of Actor Ethnicities Over Time & Figure 3.3: Distribution of Number of Cast Ethnicities Over Time](./assets/img/3.2_3.png)

In [Figure 3.3], for the first half of the century, nearly all films' casts have remained dominated by a single ethnicity, as both the average and the spread remained thin. As indicated by [Figure 3.1] above, the number of cast ethnicities follows power law distribution. [Figure 3.3] therefore measures its average across films in each decade by its geometric mean.

Since 1960s, however, the average cast ethnicity has slowly climbed, reaching 2 for the first time in 1900s and reversing its trend slightly at the turn of the century. In the backdrop of a widening spread, more and more films have joined to cast more actors from different ethnic groups during this period, with half of the films featuring actors from at least 2 ethnic groups and a quater of films featuring more than 3 since 1980s.

Although most films' casts have stayed ethnically homogeneous, there has always been some outlier films throughout history with much more ethnically diverse cast, potentially paving the way for further diversification in the future.

## 3.2 Increasing Representation: Appreciated by Audience And Reflected in Rating? 

<!-- correlation: more ethnically diverse films more well-received/higher rating
    - [ ] ethnic diversity associated/appreciated more? 

- explore cast's ethnic diversity associated with higher rating (vs influence later)
- cut-off from 1960s onwards based on spread in distribution

- generally small but positive correlation throughout
- strongest correlation at num_ethnicities >= 3 tier & 3 ethnicities as minimum threshold for an ethnically diverse cast  -->

History has shown that actors from increasingly diverse ethnic backgrounds are getting film roles and seen on the movie screens. However, are the audience appreciating this? To examine how ethnic diversity impacts a film's overall perceived quality by the audience and also how this impact has changed over time, we analyze the relationship between a film's cast ethnic diversity and its audience ratings. Tieing into the concept of 'representation', the ethnic diversity of a film is measured by the total number of different ethnicities among actors in a film's cast as seen directly by audiences on the movie screen. Film quality as perceived by the audiences is captured by the overall weighted average score of all user ratings on IMDB. As the vast majority of films consist of actors with identical ethnicity until 1950s, 1960s is chosen at the period to begin the analysis.

In general, there is a small but positive correlation between a film's cast ethnic diversity and rating. As shown in [Figure 3.4] at various levels, across decades, the more ethnically diverse the cast, the higher the film rating. This correlation, measured by the Pearson Correlation Coefficient, is the strongest at the diversity level where only films featuring actors from at least 3 different ethnic groups are considered. We therefore uses this as a threshold to split films into ethnically diverse and non-diverse groups to continue the analysis. This threshold makes sense because in a country with one dominant ethnic group, it makes sense to see at least two minority ethnic group also featured to qualify as 'diverse'.

![Figure 3.4: Correlation Between Number of Cast Ethnicity and Film](./assets/img/3.4.png)

This begs the question - does an ethnically diverse cast lead to a more highly-rated film? Let's dive in. 

## 3.3 Identifying Impact: Ethnically Diverse Cast Improves Film Rating? 

<!-- correlation: more ethnically diverse films more well-received/higher rating

    - [ ] ethnic diversity associated/appreciated more/higher correlation in recent decades? 
    - [ ] raise question: ethnically diverse cast contributes to higher rating? 

causation & significance: greater ethnic diversity in cast influence/leads to higher rating
    - [ ] expect yes in recent decades where greater ethnic representation translates to higher rating/audience appreciation 


- ethnically diverse films average rating consistently higher, with overlapping ci in 1970s and 2000s
- after pair matching, still the case: 3 statiscally significant difference in means out of 5 decades => presence of influence/causality

- however, average rating of both groups face downward trend, but ethnically diverse films rating decreases more 
- more ethnically diverse films and more ethnically non-diverse films released over the decades alike 
- => potentially because in the earlier decades, few ethnically diverse films and they are generally highly rated, then more studios started producing more films featuring diverse casts and the average rating begin to converge to overall average rating/population mean -->

After establishing treatment group of ethnically diverse films and control group of ethnically non-diverse films, their average ratings are compared in Figure X.1. Notably, films with ethnically diverse cast are rated consistently higher, with only 95% confidence interval overlapping in 1970s and 2000s. 

![Figure 3.5: Average Rating of Ethnically Diverse vs Non-Diverse Films](./assets/img/3.5.png)

After removing covariates such as release date, countries, languages and genres through propensity matching, the same still holds as ethnically diverse films consistently outperform non-diverse films in average rating in every decade. Hypothesis testing reveals that the differences in average ratings are statiscally significant in 3 of 5 decades highlighted in circles in Figure X.2. This confirms that films with ethnically diverse cast tend to be better-received by the audience and contribute to higher ratings.


![Figure 3.6: Average Rating of Pair-Matched Ethnically Diverse vs Non-Diverse Films & Figure 3.7: Number of Ethnically Diverse vs Non-Diverse Films Released](./assets/img/3.6_7.png)


However, there exists an obvious downward trend for both groups, with the average rating of ethnically diverse films decreasing faster. This does not necessarily mean that audience appreciates ethnic diversity less over time. As evidenced by Figure X.3, there is a fast-paced growth in the number of ethnically diverse films released over the decades. The decline in rating of ethnically diverse films coincide with this growth. As this number approaches and even surpasses in the last 2 decades the number for ethnically non-diverse films in the previous decades, the average rating of ethnically diverse films also closes in on that of non-diverse ones. This could potentially be because in the earlier decades, few ethnically diverse films are made and they are generally rated quite well. This possibly motivated movie studios to produce more films featuring diverse casts and with increasing volume, the average rating begin to converge to overall average rating representative of the true population mean. This would mean despite recent laudable calls in the public for greater ethnic diversity on the film set, history has shown that ethnic diversity alone does not translate to higher rating.
