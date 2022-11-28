# project1_ranking_model
basic movie ranking model

abstract:
The growing development of China’s film and television industry has brought huge market revenue.At the same time, uneven film and television dramas have also caused inconvenience to viewers. Thus,our group establish a rational ranking system based on Improved TOPSIS model.
Fristly, we crawl 250 movies from Douban and clean the raw data. Next, we do the data visulazition to descripe the data distirbution and relationship. Then we use number of votes and mean score to adjust original score to avoid malicious scoring. Again we select the adjusted score,duration,comment number and voting number to construct a movie ranking model. On the basis of the above four indicators,a comprehensive integrated weighting method combining expert evaluation method(EEM) and entropy weight method (EWM) was used to get an indicator, aiming to achieve the unity of subjective and objective in the determination of weights, after which TOPSIS is used to obtain the ranking.Finally,we compare the ranking results with the Douban official ranking and discuss the differences.
key words: Movie Ranking; Expert Evaluation Method; Entropy Weight Method;TOPSIS

data vitualization

![distibution](https://github.com/cecijia/project1_ranking_model/blob/main/photo/c903c3895acc7a0e436e8068d2b5223.png)
