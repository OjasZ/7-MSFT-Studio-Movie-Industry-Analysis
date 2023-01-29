                                               
                                            MSFT-Studio-Movie-Industry-Analysis
                                              
 Abstract:
 
Purpose: Data analytics techniques can help to predict movie success, as measured by box office
sales or Oscar awards. Revenue prediction of a movie before its theatrical release is also an
important indicator for attracting investors. While measures for predicting the success of a movie
in box office sales and awards are widely missing, this study uses data analytics techniques to
present a new measure for prediction of movies’ financial success.
Methodology: Data were collected by web-scraping and text mining. Classification and Regression
Tree (CART), Random Forests, Conditional Forests, and Gradient Boosting were used and a model
for prediction of movies' financial success proposed. Content strategy and generating high profile
reviews with complex themes can add to controversy and increase the chance of nomination for
major movie awards, including Oscars.
Findings/Contribution: Findings show that data analytics is key to predicting the success of movies.
Although predicting sales based on data available before the release remains a difficult endeavor,
even with state-of-the-art analytics technologies, it potentially reduces the risk of investors, studios
and other stakeholders to select successful film candidates and have them chosen before the
production process starts. The contribution of this study is to develop a model for predicting box
office sales and the chance of nomination for winning Oscars.


Practical Implications : Cinema managers and investors can use the proposed model as a guide for
predicting movies’ financial success.

Keywords : Media Economics; Cinema Economics; Film Financing; Hollywood Economics; Box-
Office Revenues; Data Mining; Text Mining; Movie Analytics; Oscars; Prediction Markets;
Measurement.

Introduction
The movie industry is one of the most profitable sectors of media, generating multi-billion
dollars of revenue each year. The global market reached 101 billion USD in 2019, with an 8% increase
from the previous year. The U.S market alone reached 36.6 billion USD with a 4% percent increase
from the previous year and 25% from 2015 (MPA, 2019); while it was expected to have raised to 50
billion USD in 2020 (Film Industry Statistics, 2018). The figures are a combination of cinema and
home/mobile entertainment. Such a huge market size has been created by various types of investors
who finance the production of movies and other activities in the value chain, including distribution
and exhibition. Research shows that the average investment to produce a movie is 65 million USD
(Mueller, 2011). However, the success of a movie is highly uncertain, and a large number of failed
movies reflect the risk of investment for investors. Between 2000 and 2010, only one-third of movies
in the US were profitable (Lash & Zhao, 2016). So, the prediction of movies’ performance is a critical
factor to encourage investment in the movie industry and to support growth in this market.
In addition to investors, owners of cinema theatres also face the risk of releasing unsuccessful
movies. These owners of movie theatres largely depend on box-office revenue to turn a profit, and
selecting the right movies, preferably US blockbusters, is critical for their business survival. However,
figures on revenues of movies from box office sales and home/mobile consumption are strongly
affected by market changes. The global income from box office revenues is reported as 42.2 billion
USD (down from 101 billion USD mentioned above), only increasing by 1% from the previous year.
U.S. and Canada box office revenue reached 11.4 billion USD in 2019, a decrease of 4% from 2018 and
was nearly equal to 2016 (MPA, 2019). This decline resulted in downsizing the number of cinemas.
Digital access and new ways of home/mobile consumption made downstream influenced cinema
theaters in the U.S. and the number of cinemas dropped from 7,480 in 1997 to 5,750 in 2017 (Film
Industry Statistics, 2018). This is not surprising as home viewing had been considered a major trend
in movie consumption long ago (Gomery, 2004: 202).
Other statistics support the fact that cinema owners face a decline in the number of visitors. 54%
of Americans prefer to consume the movies in their home and not to go to cinemas anymore, while
19% watch movies once a month, 8% several times a month, and only 4% of Americans buy tickets to
watch a movie in the cinema every week. The U.S. film market ranks third for box office revenues in
the world, lagging China and India (Film Industry Statistics, 2018). Such statistics reflect the economic
challenge of cinema owners in the age of digital distribution (Ulin, 2010).
The economics of the movie shows that the money generated from a film comes from a sequence
of profit or release windows. As stressed by Vogel (2014), market control is enacted by these
“windowing” practices. These come as revenue-maximization strategies of feature film exploitation
which begin their marketing life in domestic theatres and then go on to maximize revenue streams in
the ancillary markets, such as global distribution in theatrical and subsidiary markets to pay cable,
pay-per-view, commercial TV and home video (Vogel, 2014)



Materials and Methods


This study aims at forecasting box office revenues obtained during the first week of the movie
release. Such prediction is useful as cinema owners and their managers can now better decide what
movies are to be shown in their theaters. As illustrated in figure 1, the largest portion of a movie’s
revenue (40% on average) is obtained from the box office sale during the first week of a release, when
other cinema managers are yet to decide whether to show the movie or not.
Due to the importance of the cinema managers’ decision about what movie to show, we had put
ourselves in the shoes of managers to consider a real-life situation, based on all information available,
and see how we can make decisions.

Classification And Regression Tree (CART)
 
Classification And Regression Tree (CART) has been used as the first model. This technique is
an improved nonlinear and entirely non-parametric statistical learning technique first introduced by
Breiman, Friedman, Stone, & Olshen (1984). This technique enables researchers to predict a
dependent variable from independent variables. To do this, a decision tree should be built, and
graphical illustrations need to be used to interpret it. CART proceeds as follows. at each node, the
algorithm splits the dataset into two subsets, using any possible predictor and any cut-off point for
continuous predictors, in such a way that the two subsets be as homogeneous as possible concerning
the dependent variable. This technique has the advantage of being non-parametric, thus not
postulating any a priori assumption on the distribution of the data, being robust to outliers, and
supporting all types of variables. Also, the CART algorithm effectively handles missing values. When
the learning sample is as large as in the present case for most reference periods, the CART algorithm
has properties that are similar to the nearest neighbor algorithm. On the other hand, limitations
include the inability to detect combinations of variables as effective predictors, and the need for a
large sample (which may be problematic for the period 2010-2012 and 2011-2012).

Results of four models

The results of each of the four above-mentioned models are presented in Table 9. It shows that
regardless of the estimation method, an increase in the number of observations that serve as reference
leads to an increase in the R-square; therefore, the use of more movies to construct the model does
better explains the variance. The results are similar when using movies released between 2000 and
2012 or those released between 2006 and 2012 (the best-explained variance of 79% is for this latter
period). Therefore, arguably, our optimal time range of films to be considered for estimation is 6 years
(with a preference for the 2006-2012 range), if we wanted to maximize the explained variance.
Random forests, conditional forests and gradient boosting seem to be the three methods giving
marginally better results. This makes sense given their complexity. However, the difference in
performance between the best models and classical linear regression remains marginal.
For obtaining higher coefficients of determination, other variables that indicate quality
expectations of movies are needed. Neither use nor cinema managers have access to such
information. Root Mean Square Error (RMSE) is large, (10 million US dollars in January 2010), and
the average error rate is very high too, between 596.99% to 22.30%. Such figures are due to the
presence of extreme values and explain the reason why the use of Root Median Square Error and the
median error rate for this matter. Since the RMSE fluctuated between 110,000 and 2,000,000 USD, the
indicators of predictive power are preferable. These indicators support the idea that Random Forests
and Gradient Boosting are the best models.

Conclusions

Early prediction of movie performance is critical for investors, film producers, cinema owners
and other stakeholders in film exploitation. Considering a large amount of required investment to
produce a movie, the risk of investing in a failed product is significant. For this reason, research has
been conducted to develop models for prediction of movies' success to assist the stakeholders in their
decision-making.

Here it is explained models to predict box office revenue for movies by the set of variables
identified, and then discussed how these could correlate with Oscars awards. It could also be shown
that data analysis is key to predicting movie success and hence may reduce the risk of investors as
well as cinema owners to select the right movies in advance.
