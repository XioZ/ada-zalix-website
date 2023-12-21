# Team ZALIX Milestone 3

# An Evolutionary View on The Making of Good Films

Embark on a captivating journey through the movie industry as we delve into the heart of the movie industry—a powerhouse shaping global economics and enriching our lives. With a myriad of films flourishing, the quest for quality has intensified, leading to the establishment of renowned rating systems like IMDb, a cinematic authority.

Join us in unraveling the essence of a compelling film and exploring its various facets that contribute to cinematic excellence. This project invites you to take a ride through the annals of movie history, tracing the evolution of people's perceptions of what constitutes a "good film." So fasten your seatbelts and immerse yourself in an adventure that navigates the captivating landscape of cinematic evolution.

In order to do this , we will investigate 
1. The Impact of genre and runtime on the films rating, the evolution of perception of genres over time.
2. Are there any sweet spots or patterns in the length of top-rated films over the years? Is there a significant difference in the length of good movies across genres?
3. How has the global actor demographics changed over time in terms of ethnic background, gender and languages spoken? Does the demographic shift translate to more ethnically, gender and linguistically diverse movies produced over the years? More importantly, is a more ethnically, gender and linguistically diverse cast appreciated by the audience and directly contribute to higher movie ratings?
4. The presence of star translate to higher ratings ? How has the impact of stars evolved over time in movie ratings?

We have established a criterion for highly-rated movies, considering those with a rating surpassing 7. This threshold is set at approximately one standard deviation above the mean of average ratings, providing a robust benchmark for cinematic excellence.

# 1. Genre 
To begin with, let us take a look into __genres__, which play a crucial role in defining the stylistic and thematic elements that shape a film's identity. Unlike strict boundaries, many movies embrace a blend of genres, creating a rich tapestry of storytelling that transcends traditional categorizations. From action-packed adventures with a touch of romance to thought-provoking science fiction infused with elements of comedy, the interplay of multiple genres adds layers of complexity and intrigue to cinematic experiences. Whether it's a thrilling action-comedy, a romantic fantasy epic, or a crime drama with elements of mystery, the fusion of genres allows filmmakers to craft narratives that appeal to a diverse audience, offering a dynamic and ever-evolving landscape within the world of cinema.

In our evaluation of cinematic quality, the role of genres in influencing ratings emerges as a noteworthy consideration. The objectives of this analysis encompass the exploration of various research questions:

- Identification of the top 10 most prolific genres in the history of cinema.
- Evaluation of the proportion of exemplary films within the aforementioned 10 most prolific genres.
- Examination of the intersection between genres and the temporal variable, aiming to identify "golden eras" marked by periods with the highest number of highly-rated films within a specific genre. This will be accomplished through the visualization of highly-rated movie counts per decade.
- Scrutiny of genre combinations to discern noteworthy amalgamations during specific time periods. This aspect of the analysis will involve the generation of a bar chart illustrating the ratio of highly-rated movies relative to each decade.

## 1.1 Most Prolific: Top 10 Genres in The History of Cinema
{% include 1-1.html %}

Upon examination of the aforementioned graph, it becomes evident that there are over 700 genres, with a considerable portion having a minimal number of movies, rendering them inconsequential for our analytical purposes. Consequently, we have elected to narrow our focus to the top ten genres, as they not only serve as more representative subsets but also encapsulate the majority of films within our dataset.

![Figure 1.2: Number of Movies for the Top 10 Genres](./assets/img/1.2.png)

![Figure 1.3: Percentages of Number of Movies for the Top 10 Genres](./assets/img/1.3.png)

Given that our criterion for categorizing "good" movies hinges on those with a rating surpassing 7, we proceed to implement a filtering mechanism. This entails narrowing our focus exclusively to movies meeting this specific high-rating threshold. By concentrating on this subset of films, we aim to glean more targeted insights into the characteristics and trends associated with movies that align with the established criteria for excellence.

![Figure 1.4: Number of High-Rating Movies for the Top 10 Genres](./assets/img/1.4.png)

The graphical representation highlights the prominence of the __Drama__ genre, possessing the highest count of highly-rated movies, a figure significantly surpassing other genres. However, it is imperative to consider that the sheer abundance of drama films in the dataset could contribute to this observation. To delve deeper into the matter, we meticulously examine the ratio of high-rated movies to the total number of movies within each genre, providing a more nuanced perspective on the prevalence of quality content within the diverse genres.

![Figure 1.5: Ratio of High-Rating Movies to the Total Number of Movies per Genre](./assets/img/1.5.png)

The graph reveals noteworthy insights into the distribution of highly-rated movies across genres. Notably, __Short Films__ exhibit the highest ratio of highly-rated movies to the total number of short films, positioning it at the forefront. __Drama__, despite its prominence in sheer numbers, takes the second position in this ratio analysis. Conversely, __Adventure__ and __Action__ genres exhibit the lowest ratios, indicating a comparatively lower prevalence of highly-rated movies within these genres. This nuanced examination contributes to a more comprehensive understanding of the quality distribution across various film genres.

## 1.2 Genre Appeal: The Lure of Some Genres To Critics' Eyes 

Subsequently, we incorporate the temporal variable into our analysis to explore whether certain genres exhibit a notable concentration of highly-rated movies during specific time periods. The objective is to discern if there are temporal intervals wherein a particular genre experiences a significantly higher count of highly-rated movies compared to other periods. This temporal analysis aims to uncover patterns and trends in the distribution of high-quality movies within individual genres across different epochs.

{% include 1-6.html %}

The graphical representation highlights two notable surges in the number of highly-rated movies throughout history: __one during the 1930s and another in the 2000s__.  During these intervals, there is a pronounced surge in the number of movies receiving high ratings. Intriguingly, in the aftermath of both periods, there is a noticeable decline, coinciding with two significant economic crises—the Great Depression in the 1930s and the global financial crisis of 2008. The observed correlation between economic downturns and fluctuations in the production and reception of high-quality movies prompts an exploration into the intricate dynamics at play during times of economic instability. Unraveling the contextual factors influencing these trends can provide valuable insights into the evolving landscape of the film industry across different historical epochs.

The analysis of the graphical representation yields several noteworthy insights. Firstly, **Comedy** and **Romance Film** emerge as the most popular highly rated genres, with a notable surge in popularity since the 1960s. Secondly, genres such as **Thriller**, **Crime Fiction**, and **Indie** films exhibit a rising trend in popularity. Thirdly, there is a distinctive surge in the prevalence of highly rated **Short Films** at the onset of the 21st century. Lastly, despite an overall increase in the number of films, **Adventure** and **Action** genres consistently exhibit a lower proportion of high-rated movies.

Now, let's dig deeper into the __Drama__ genre to examine the impact of its combinations with other genres.

{% include 1-7.html %}

From the aforementioned analysis, we observe a similar trend as in the overall analysis. It is noteworthy that __Romance Films__ and __Comedies__ are the most popular genres when combined with Drama. Additionally, the combination of __Short Films__ and __Drama__ gains popularity particularly after the year 2000. The coherence in trends underscores the dominant influence of the Drama genre in highly rated movies.


![Figure 1.8: Number of Black-and-White and Romance Movies for Each Past Decade](./assets/img/1.8.png)

![Figure 1.9: Number of Black-and-White and Romance Movies for Each Past Decade](./assets/img/1.9.png)


It comes as no surprise that a significant proportion of highly-rated movies in black-and-white were made during the 1940s, with a notable concentration within the drama genre. This observation underscores the enduring appeal of the black-and-white aesthetic in conveying the nuanced themes often associated with dramatic narratives. Furthermore, within the realm of black-and-white films, the comedy and romance genres emerge as particularly prominent, constituting the majority of high-rated movies. This alignment suggests a unique intersection of visual style and storytelling elements that contribute to the success and acclaim of black-and-white comedies and romances. A more in-depth exploration of these specific films can shed light on the distinctive qualities that make them stand out within the broader landscape of high-quality cinema.

Delving into the significant surge observed in the 2000s, we aim to meticulously examine the intricate effects resulting from combinations of genres during this prolific period. By scrutinizing the interplay between different genres within this temporal frame, we seek to unravel patterns, preferences, and potential synergies that contributed to the remarkable increase in the number of highly-rated movies. This focused analysis on genre combinations promises to unveil insights into the evolving tastes, creative trends, and collaborative dynamics that defined the cinematic landscape during this particular era, enriching our understanding of the multifaceted factors influencing the success of movies.

{% include 1-10.html %}

![Figure 1.11: Percentage of number of Movies after 2000](./assets/img/1.11.png)

From the comprehensive analysis presented above, a discernible trend emerges, indicating that the __Drama__ genre has consistently dominated the cinematic landscape. This dominance is reflected in both the largest number of total movies across all genres. The enduring popularity and prevalence of drama underscore its universal appeal, serving as a versatile and enduring vehicle for storytelling that resonates with diverse audiences. As we continue to explore the intricacies of genre dynamics, the prominence of drama stands as a testament to its enduring significance within the ever-evolving world of cinema.

## 1.3 Topic Analysis: Well-Liked Topics Among Top Genres

After identifying the most 'liked' genres based on the highest-ranked movies, we plan to conduct topic analysis using the LDA algorithm on the plot summaries of these top-ranked movies. Our objective is to define the most liked topic within each of the top 5 most preferred genres. The following outlines the interpretation of the topics generated by the LDA algorithm:

## Drama

**Family and Personal Struggles:** This topic focuses on themes like life, love, family dynamics, and personal challenges. It often involves characters dealing with complex relationships and emotional journeys.

**Crime and Conflict**: This topic is centered around police, crime, murder, and gang-related activities. It often includes elements of suspense, betrayal, and moral dilemmas.

**Historical and Political Drama:** Involving films with themes like war, leadership, and national issues. It may include movies about historical figures, soldiers, and significant political or social events.

## Comedy

**Romantic and Family Comedy:** This topic deals with love, friendship, and social life. It often includes humorous takes on relationships, family, and everyday situations.

**Dark Comedy:** Includes comedic films that may parody other genres or societal norms. It involves elements like police, money, and life's absurdities.

**Adventurous and Escapades:** Focuses on characters like Jack and themes of adventure, road trips, and escapades, often with humorous undertones.

## Short Film

**Adult Films:** This topic is about short films that focus on storytelling and character development, often involving personal tales and life experiences.

**Animated Classics and Characters:** Centers on classic animated characters like Ralph, Sylvester, Tweety, and the Pink Panther, often involving comedic and adventurous plots.

**Adventurous and Escapades:** Involves characters in constant motion, like Wile E. Coyote and Road Runner, featuring physical comedy and slapstick elements.

## Black-and-White

**Classic Storytelling:** Involves traditional narrative structures with elements of suspense, resolution, and often a moral lesson.

**Character-Centric Tales:** Focuses on personal stories and relationships, often involving a journey or transformation of the main characters like Mary or Tramp.

**Family and Life Journeys:** Deals with themes of love, life, home, and the passage of time, often exploring deep emotional and relational aspects.

## Romance Film

**Modern Love and Relationships:** This topic explores contemporary romantic relationships, often set in urban environments and involving themes of love, career, and personal growth.

**Royal and Aristocratic Romance:** Involves stories about royalty and aristocracy, with characters like kings, princes, and their romantic and political intrigues.

**Family Romance:** Centers on timeless themes of love and life, often involving family dynamics, personal discovery, and the evolution of relationships over time.

![Figure 1.12: Topic distribution within the top 5 most preferred genres](./assets/img/1.12.png)

We notice that the family topic is common within all the genres with a significant percentage. This suggests that the family tocpic might have an influcence with the good ranking of movies, therefore might be within the most appreciated topics by the film public.

# 2. Length 

## 2.1 Lengthy Films: Eliminating Bias from Excessively Long Films

The length of a film, a fundamental element in cinematic storytelling, serves as a crucial factor influencing the overall viewing experience and perceived quality. Film durations vary widely, ranging from concise short films to sprawling epics. The impact of a movie's duration on its quality is a nuanced consideration that intertwines with storytelling techniques, pacing, audience engagement, and thematic depth. A well-crafted film can leverage its duration to immerse viewers in its narrative world, allowing for character development, plot intricacies, and emotional resonance. However, an excessively long or brief duration may pose challenges, potentially leading to pacing issues or insufficient exploration of complex themes. This intricate interplay between movie duration and quality underscores the significance of understanding how filmmakers navigate the temporal dimension to create compelling and impactful cinematic experiences.

![Figure 2.1: Distribution of movie runtime before removal of outliers](./assets/img/2.1.png)

Upon examination of the graph presented above, a noteworthy pattern emerges where a considerable number of films exhibit either exceptionally short or excessively long durations, exceeding 5000 minutes. To ensure the precision and reliability of our analysis, it is imperative to address these outliers. Eliminating such extreme values is essential for a more accurate representation of the dataset and will contribute to the robustness of our findings.

Additionally, it is pertinent to acknowledge that short films often have relatively brief durations, which could potentially skew our analysis of runtime for regular feature-length movies. Fortunately, a substantial portion of these short films falls within the category of outliers slated for removal. This strategic refinement of the dataset aims to enhance the integrity of our examination of movie durations and facilitate a more nuanced understanding of the temporal aspects within the cinematic landscape.

![Figure 2.2: Distribution of Movie Runtime after Removal of Outliers](./assets/img/2.2.png)

## 2.2 Regression Analysis: Longer Runtime Means Higher Rating?

![Figure 2.3: Regression of Movie Runtime with Respect to Average Rating](./assets/img/2.3.png)

The preliminary regression analysis indicates a noteworthy trend where longer durations tend to correlate with higher average ratings. This initial observation prompts further investigation to validate and refine our understanding of the relationship between movie duration and audience ratings. While this finding suggests a positive association, additional factors such as genre, thematic content, and storytelling techniques may contribute to a more nuanced interpretation. Therefore, a more in-depth and comprehensive analysis is warranted to ensure a robust understanding of the intricate dynamics influencing movie ratings in relation to their durations.

{% include 2-3.html %}

Our analysis adopts a dual perspective, delineated by two distinct criteria. Firstly, the dataset is bifurcated based on ratings, with a division into two halves. Subsequently, the dataset is segregated based on duration, categorizing movies with a runtime exceeding 80 minutes as long-duration films. Two sets of t-tests are conducted to discern potential statistically significant differences: one examines the mean average duration between high-rating and lower-rating movies, while the other investigates the mean average rating between long-duration and shorter-duration movies. These parallel analyses offer a comprehensive exploration of the interplay between movie ratings, durations, and their potential impact on cinematic characteristics.

Conducting a t-test on the runtime variable is imperative to ascertain the presence of a statistically significant distinction between two subsets of movies based on their ratings. Specifically, this analysis aims to discern whether there exists a noteworthy difference in runtime duration between movies with ratings exceeding 7 and those with ratings below 7. By rigorously applying statistical methods, we endeavor to illuminate any discernible patterns or variations in movie runtimes associated with differing rating categories.

{% include 2-4.html %}

Based on the preceding analysis, it is evident that a statistically significant difference exists between the means of movie runtimes for those with ratings exceeding 7 and those with ratings below 7. The mean duration of high-rating movies is found to be 7.71% higher than that of their lower-rated counterparts. This finding suggests a notable variation in runtime characteristics between movies of distinct rating categories, emphasizing the potential influence of audience ratings on the temporal aspects of cinematic storytelling.

{% include 2-5.html %}

Based on the outcomes of the t-test, it is evident that a statistically significant difference exists in the means of average ratings between long-duration movies and shorter-duration movies. Specifically, long-duration movies exhibit a higher mean rating of 6.19, contrasting with the mean rating of 6.03 observed for shorter-duration movies. This finding underscores a notable association between the temporal extent of movies and audience ratings, suggesting that longer-duration films tend to garner higher average ratings compared to their shorter-duration counterparts.




# 3. Ethnic Diversity

Hollywood, and many major film studios around the world, has long faced criticism for the lack of racial diversity in its workforce both on and off the screens. In recent decades, there has also been a growing call for greater representation of racial minorities on the silver screen. [Figure 3.1] shows a quick exploratory analysis of the distribution of the number of ethnicities among cast members of each film between 1900 to 2009. As shown in the figure, the curve of films rated 7 or above is largely above that of films rated below. This suggests that highly rated films generally have more ethnically diverse casts than those lower rated, and cast ethnic diversity could be an interesting angle to further our investigation. 

![Figure 3.1: CCDF of Number of Cast Ethnicities in High-Rating vs Lower-Rating Films](./assets/img/3.1.png)

## 3.1 Shifting Demographics: From Diverse Actors Pool To Diverse Casts

To set the stage, let's first take a look at how the ethnic demographics of actors has evolved globally over time. [Figure 3.2] shows that the 110-year history of film-making has witnessed a booming growth in the ethnic background of actors, with the trend accelarating after 1960s.

This fast diversifying shift in the acting workforce is reflected on the silver screen, through greater, though much more subdued, ethnic representation by the collective featuring of actors from different ethnic backgrounds in the same films.

![Figure 3.2: Number of Actor Ethnicities Over Time & Figure 3.3: Distribution of Number of Cast Ethnicities Over Time](./assets/img/3.2_3.png)

In [Figure 3.3], for the first half of the century, nearly all films' casts have remained dominated by a single ethnicity, as both the average and the spread of the number of ethnicities among cast per film remained thin. As indicated by [Figure 3.1] above, the number of cast ethnicities follows power law distribution. [Figure 3.3] therefore measures its average across films in each decade by geometric mean.

Since 1960s, however, the average cast ethnicity has slowly climbed, reaching 2 for the first time in 1900s and reversing the trend slightly at the turn of the century. In the backdrop of a widening spread, more and more films have joined to cast more actors from different ethnic groups during this period, with half of the films featuring actors from at least 2 ethnic groups and a quarter of films featuring more than 3 since 1980s.

Although most films' casts have stayed ethnically homogeneous, there has always been some outlier films throughout history with much more ethnically diverse cast than their contemporaries, potentially paving the way for further diversification in the future.

## 3.2 Increasing Representation: Appreciated by Audience And Reflected in Rating?

History has shown that actors from increasingly diverse ethnic backgrounds are getting film roles and seen on the silver screen. However, does the audience consider a film with a more ethnically diverse cast a better film? To examine how ethnic diversity impacts a film's overall perceived quality by viewers and also how this impact has changed over time, we analyze the relationship between a film cast's ethnic diversity and its audience ratings. Tying into the concept of 'representation', the ethnic diversity of a film is measured by the total number of different ethnicities among actors in a film as seen directly by the audience on a movie screen. Film quality as perceived by the audience is captured by the overall weighted average of all user rating scores on IMDB. As the vast majority of films consist of actors with identical ethnicity until the 1950s, the analysis begins with the 1960s.

In general, there is a small but positive correlation between a film's cast ethnic diversity and rating. As shown in [Figure 3.4] at various levels, across decades, the more ethnically diverse the cast, the higher the film rating. 

![Figure 3.4: Correlation Between Number of Cast Ethnicity and Film](./assets/img/3.4.png)

This correlation, measured by the Pearson Correlation Coefficient, is the strongest at the diversity level where only films featuring actors from at least 3 different ethnic groups are considered. We therefore uses this as a threshold to split films into ethnically diverse and non-diverse groups to continue the analysis. This threshold makes sense because in most countries where there is one dominant ethnic group, 'diverse' should mean seeing at least two minority ethnic groups featured as well. This begs the question - does an ethnically diverse cast contribute to a more highly rated film? Let's dive in. 

## 3.3 Identifying Impact: Ethnically Diverse Cast Improves Film Rating?

After establishing a treatment group of ethnically diverse films and a control group of non-diverse films, their average ratings are compared in [Figure 3.5]. Notably, films with ethnically diverse cast are rated consistently higher, with the 95% confidence interval overlapping only in the 1970s and 2000s. 

![Figure 3.5: Average Rating of Ethnically Diverse vs Non-Diverse Films](./assets/img/3.5.png)

An observational study is conducted to disect this claim. Logistic regression is carried out using data from both groups and takes observed confounders as features, including release date, countries, languages and genres. The regression model calculates each film's probability to have an ethnically diverse cast. Propensity matching is then performed in each decade, to pair match similar films from both groups. After removing covariates through pair matching, [Figure 3.6] reveals that the claim still stands, as ethnically diverse films consistently outperform non-diverse films in average rating. Hypothesis testing shows that the difference in average ratings is statistically significant in 3 of the 5 decades, which are highlighted in circles. This confirms that films with an ethnically diverse cast tend to be better-received by the audience, and ethnic diversity among cast members contributes to higher ratings.


![Figure 3.6: Average Rating of Pair-Matched Ethnically Diverse vs Non-Diverse Films & Figure 3.7: Number of Ethnically Diverse vs Non-Diverse Films Released](./assets/img/3.6_7.png)


However, there exists an obvious downward trend for both groups, with the average rating of ethnically diverse films decreasing faster. This does not necessarily mean that audience appreciates ethnic diversity less over time. As evidenced by [Figure 3.7], there is a fast-paced growth in the number of ethnically diverse films released over the decades. The decline in rating of ethnically diverse films coincides with this growth. As this number approaches and eventually surpasses in the last 2 decades the number of ethnically non-diverse films in the previous decade, the average rating of ethnically diverse films closes in on that of non-diverse ones. This could potentially be because in the earlier decades, few ethnically diverse films are made, and they generally end up well-received and highly rated. This possibly motivates movie studios to produce more films featuring diverse casts and with increasing volume, the average rating begins to converge to the average rating representative of the true population mean overall. This could mean that despite recent laudable calls in the public for greater diversity on the film set, history has shown that ethnic diversity alone does not translate to higher rating.

# 4. Stars 

The correlation between star power and ratings in the movie industry has long been a subject of fascination. Over the years, the influence of A-list actors and actresses on the success of a film has undergone a significant evolution. The captivating question persists: does the presence of renowned stars inherently lead to higher ratings? How has the impact of stars evolved over time in movie ratings? 

## 4.1 Star-Studded Success: How Movie Stars Shine on Film Rating
We aim to explore the correlation between star actors and movie ratings through a linear regression analysis. Specifically, we investigate how each actor contributes to the overall movie ratings.

To ensure a robust analysis, we focus on actors who have participated in a minimum of 35 movies, thereby isolating those with a substantial presence in the industry.

By retaining only coefficients with p-values < 0.05, we guarantee the statistical significance of the data, ensuring meaningful results.

![Figure 4.1 Impact On Movies Ratings by Star Actors](./assets/img/4.1.png)

It is crucial to note that, initially, the linear regression yielded a modest R-squared value of 0.1. This indicates that using actors alone poorly explains the variability in movie ratings. Nevertheless, the regression identified 14 actors whose contributions significantly impact movie ratings.

Movies featuring actors such as Bette Davis or Mel Blanc demonstrate a noteworthy boost of nearly one point in their ratings due to their involvement.


# 5. Conclusion
Finally, after a wonderful jouney, we arrived to the conclusion of that Drama genre is widely praised for its high quality among the past decades, especially when combined with Romantic themes. The high-rating movies ubiquously have a duration longer than 80 minutes and this is the sweet spot that people generally like.
