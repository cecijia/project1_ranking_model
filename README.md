# project1_ranking_model
basic movie ranking model

# abstract:
The growing development of China’s film and television industry has brought huge market revenue.At the same time, uneven film and television dramas have also caused inconvenience to viewers. Thus,our group establish a rational ranking system based on Improved TOPSIS model.
Fristly, we crawl 250 movies from Douban and clean the raw data. Next, we do the data visulazition to descripe the data distirbution and relationship. Then we use number of votes and mean score to adjust original score to avoid malicious scoring. Again we select the adjusted score,duration,comment number and voting number to construct a movie ranking model. On the basis of the above four indicators,a comprehensive integrated weighting method combining expert evaluation method(EEM) and entropy weight method (EWM) was used to get an indicator, aiming to achieve the unity of subjective and objective in the determination of weights, after which TOPSIS is used to obtain the ranking.Finally,we compare the ranking results with the Douban official ranking and discuss the differences. <br>
<br>
key words: Movie Ranking; Expert Evaluation Method; Entropy Weight Method;TOPSIS

# data vitualization

## Distribution of movies released in different countries

The warmer the colour is, the more excellent movies are issued in that country <br>
The United States has 137 excellent movies<br>
China has 63 excellent movies<br>
The United Kingdom and Japan are in the third and fourth place<br>
![map](https://github.com/cecijia/project1_ranking_model/blob/main/photo/map-world2-0.cx7ihfmh95r-1.jpg)

## Violin chart of score, duration and number of comments

The score of movies is concentrated at 8.8 <br>
The duration of movies is concentrated between 90 and 130 minutes <br>
The number of comments for movies is concentrated between 8,000 and 12,000<br>
![distibution](https://github.com/cecijia/project1_ranking_model/blob/main/photo/c903c3895acc7a0e436e8068d2b5223.png)

## Type and Release Year Relevant
Horizontal bar——the number of movies in different types <br>
Vertical bars——different score ranges <br>
Central plot area—— the darker the squares are, the more movies are in this area <br>

![image](https://github.com/cecijia/project1_ranking_model/blob/main/photo/score_type1.png)

## Variables Correlation
Release year<br>
Duration<br>
Number of comments<br>
Number of score<br>
No significant correlation could be found between duration, number of comments and score<br>
![image](https://github.com/cecijia/project1_ranking_model/blob/main/photo/scatter_metrix.png)

# Movie Ranking Model

use Bayesian average to modified the score
![image](https://user-images.githubusercontent.com/117010692/204245569-82c0f6bf-8808-4f54-b5e6-f7c662018dc2.png)
![image](https://user-images.githubusercontent.com/117010692/204245705-af7dfaa6-92e1-4b12-b620-6399af864848.png)
<br>
the weight derived from EWM represent the objective weight and the other(AHP/CRITIC/EEM) one refers to the subjective weight.



# Model Implementation

# conclution
Based on previous analysis, we found that drama films had a higher rate of high scores. At the same time, based on main type and subtype, we found that some themes always appear in bundles, such as romance and comedy elements often appearing in the drama genre. A comprehensive TOPSIS rating system was established by selecting film score, duration, number of votes and number of comments as the main indicators, and re-ranking 250 films on Douban, and the results show that the model is highly generalisable.

# Strengths and Weaknesses
## Strengths
The data are objective and have high universality<br>

Malicious scoring and unhealthy competition in the industry  are taken into account <br>

Comprehensive integrated weighting method<br>

## Weaknesses
Only some factors are selected to get the rankings of movie, which may affect the results to some extent.









