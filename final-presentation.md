theme: Fira, 2
autoscale: true

# [fit] Insights into **Social Media** Data: 
# [fit] a new formalism inspired in **Thermodynamics**

![](assets/thermo.jpg)

---

![](assets/intro.png)

---

[.list: alignment(left)]

## Agenda

1. **Background**
	* Literature and motivation
2. **Methodology**
	* Aims and Objectives
	* Tools and methods used
3. **Findings**
	* Analysis results
	* Discussion

![right 50%](assets/time.png)

---

![](assets/books.jpg)

# Background
# *![inline 60%](assets/background.png)*

---

[.list: alignment(left)]

# Social Media Usage

* Of the world's ~4.5 billion internet users, **~3.5 billion use social media**<sup>1</sup>
* From 2005-2015 **social media usage rose 10x** in the US alone<sup>2</sup>
* **Hundreds of platforms**, growing by the year<sup>3</sup>, most use two or more<sup>4</sup>
* Many count users in the millions, with some reaching **> 1 billion users**<sup>2</sup>
* Social media usage spans demographics<sup>5</sup>; includes individuals, groups and businesses of all sizes<sup>6</sup>
* Critical to maintaining a competitive edge in business<sup>7</sup>
* Has fundamentally **changed the way humanity communicates**<sup>8</sup>

^ Social media usage has seen some phenomenal growth over the years, with now an approximated more than three-quarters of internet users worldwide being present on social media. 

^ It's had great impact on how we view society, do business and communicate with one another.

---

[.list: alignment(left)]

# Social Media Analysis

* Understand the network structure of platforms, how people connect (**social network analysis**, **behavioural research**)
* Understand the content being generated and shared among platforms, how people react to and propagate it (**content and sentiment analysis**, **information diffusion theories**)
* Understand where particular interest comes from, the determinants and effects of popular topics (**topic analysis**, **trend analysis**)

---

[.list: alignment(left)]

# Challenges

* Social media generates content of **enormous quantity** at great speed<sup>10</sup>
* **Semi-structured** data that often includes **mixed media** necessary to context<sup>11</sup>
* Metadata is sparse + **not always accurate**<sup>12</sup>
* Hardest of **NLP**—jargon, context- + culturally-specific terms<sup>13</sup>
* **Data is harder to get** over time due to platforms commoditising data<sup>14</sup> + increasing privacy controls<sup>15</sup>

---

# [fit] Trend Analysis & "Prediction"

# ![40% inline](assets/trends.png)

![](assets/stocks.jpg)

---

![](assets/umbrella.png)

---

[.list: alignment(left)]

# Why? 

* Optimise marketing and outreach campaigns
* Understand content consumption
* Observe cultural change over time
* Jump on bandwagons
* Prevent impending harmful content trends

---

[.list: alignment(left)]

# Challenges

* Subjectivity of viewing, sharing content
* False positives in anomaly detection-based methods<sup>16</sup>
* Reliance on other information sources in alternative methods<sup>17</sup>
* Timeliness requirements for analysis and detection<sup>18</sup>
* Topic evolution over time<sup>19</sup>
* Predicting the future?

---

![](assets/pipelines.png)

---

[.list: alignment(left)]

# Multidisciplinary challenges

* Very human data; erratic behaviours (**behavioural science**)
* Sharing between non-fully-connected graph structure... (**graph theory**)
* ...of nodes with varying levels of transmissiveness (**social contagion**)
* Different content and sentiments get shared in different ways (**information diffusion**)

---

![](assets/curve.jpg)

### _"Social media analysis requires some new ways of thinking!"_[^*]

[^*]: see 15, 20-22

---

[.list: alignment(left)]

## Novel cross-disciplinary applications

* Social media trends as contagion theory from **Virology** in Medicine<sup>23 - 25</sup>
* Social media trends as the **Technology Adoption** curve from Information Diffusion Theory<sup>26</sup>
* Social media behaviours observed as sound (**Data Sonification**) to aid in anomaly detection<sup>27</sup>
* Social media network interactions as **Evolutionary Game Theory** from Evolutionary Biology<sup>28</sup>

---

[.text: #423347]
[.footer: **Source: Mahbub, de Souza and Williams 2016**]
[.footer-style: alignment(left)]

![](assets/proposal.png)

---

## Entropy Theory

![](assets/galaxy.jpg)

---

![](assets/maths.png)

---

[.list: alignment(left)]

# Entropy over time

* Reveals descriptive statistical measures about a set of data
* But also measures internal diversity and inconsistency
* Takes focus away from upper and lower bounds—or even ranges—in favour of changes in internal distribution that may be more informative
* Is in some cases sufficient to adapt analysis into Markov-model-based prediction

---

## Aims & Objectives

![](assets/target.jpg)

---

[.list: alignment(left)]
[.footer: *In that it could achieve earlier detection than existing early detection methods.]

# Broadly

1. Can the analogous application of **Entropy Theory** present useful information about the lifetime of a trend or topic on a Social Media platform?
2. Is there indication that the method could be applied more broadly, or adapted to be **predictive**?*

---

[.list: alignment(left)]

# In this study

Experimentation aimed to confirm dual hypotheses:

1. **increasing entropy over time** may suggest impending critical interest preceding a trend developing to significance, and
2. **decreasing rate of entropy increase over time** after a high entropy or engagement level has occurred may suggest new evolution in the topic.

---

[.list: alignment(left)]
[.header: alignment(left)]

# This required

* data from social media platforms,
* covering concise topics,
* for significant periods of time, with
* sufficiently varied trend behaviours and
* consistent measures of engagement.

---

![](assets/research.jpg)

# Methodology

# *![inline 60%](assets/method.png)*

---

[.list: alignment(left)]

# Process

1. Identifying Data
2. Retrieving Data
3. Preparing Data
4. Analysing Data

![right](assets/process.png)

---

[.background-color: #ff0000]
# Identifying Data

---

[.background-color: #ff0000]
Why Twitter?

---

[.background-color: #ff0000]
# Retrieving Data

---

# Hydration Loss

| **Data Group** | **Listed** | **Hydrated** | **Lost** |
|:---|---:|---:|---:|
| Hurricane Harvey | 18,336,283 | 13,018,265 | 5,318,018 |
| Hurricane Irma | 17,227,935 | 11,627,130 | 5,600,805 |
| Immigration Travel Ban | 16,842,329 | 11,618,463 | 5,223,866 |
| Winter Olympics | 13,787,299 | 10,567,141 | 3,220,158 |
| Hurricane Florence | 7,756,856 | 6,432,696 | 1,324,160 |
| Women's March | 7,263,988 | 4,526,921 | 2,737,067 |
| Ireland Vote | 2,276,808 | 1,784,345 | 492,463 |
| **Total** | **83,491,498** | **59,574,961** | **23,916,537** |

---

[.background-color: #ff0000]
# Preparing Data

---

[.background-color: #ff0000]
# Analysing Data

---

[.background-color: #ff0000]

---

![](assets/findings.jpg)

# Findings

# *![inline 60%](assets/findings.png)*

---

[.background-color: #ff0000]
* Rehash aims

---

[.background-color: #ff0000]
* Results

---

## It didn't work.

---

[.background-color: #ffffff]
![](assets/variation.png)

---

[.background-color: #ff0000]
Demonstration of it not working

---

* **Why** didn't it work?
* What does it not working **imply**?

---

[.background-color: #ffffff]
[.header: #423347]

# [fit] Data was sparse ⇒ dramatically left-skewed

![inline](assets/distplot.png)

---

[.list: alignment(left)]

# Entropy

* Range of datapoints
* Volume of datapoints
* Internal distribution

---

[.list: alignment(left)]

# Entropy

* ~~Range of datapoints~~ (made redundant)
* Volume of datapoints (inflated)
* Internal distribution (heavily weighted towards range lower bound)

^ Only dramatic changes in distribution reflected, negating predicted responsiveness

---

[.background-color: #ff0000]
Why couldn't this be accounted for?

---

[.background-color: #ff0000]
* Discussion

---

[.background-color: #ff0000]
* Hypotheses aside, could this be useful?

---

[.list: alignment(left)]

# Observed generalisations

* Entropy was **higher** during periods of growth
* Entropy **varied more** during periods of growth
* Entropy over time **increase sped up** during periods of growth

---

* No apparent prediction capabilities 👎
* Potential computationally inexpensive way to describe current behaviours 👍

---

[.background-color: #ff0000]

---

# [fit]Thanks for listening!

![](assets/fireworks.jpg)

---

[.text: alignment(left)]

# References

<sup>1</sup> Hootsuite: 2018, Hootsuite’s social media barometer report. [https://hootsuite.com/resources/all-future_of_social-digital_in_2019-glo-en-ca-digital_in_2019-q1_2019](https://hootsuite.com/resources/barometer-2018-global?utm_campaign=all-future_of_social-digital_in_2019-glo-en-ca-digital_in_2019-q1_2019) [Accessed 18 May 2018].
<sup>2</sup> Perrin, A.: 2015, Social media usage: 2005-2015, _PEW Research Center Report_.
<sup>3</sup> Kasemsap, K.: 2019, Professional and business applications of social media platforms, Social Entrepreneurship: Concepts, Methodologies, Tools, and Applications, _IGI Global_, pp. 824– 847.
<sup>4</sup> Zhao, X., Lampe, C. and Ellison, N. B.: 2016, The social media ecology: User perceptions, strategies and challenges, _Proceedings of the 2016 CHI conference on human factors in computing systems_, ACM, pp. 89–100. 
<sup>5</sup> Kane, G. C.: 2015, Enterprise social media: Current capabilities and future possibilities., _MIS Quarterly Executive_ 14(1). 
<sup>6</sup> Kaplan, A. M. and Haenlein, M.: 2010, Users of the world, unite! the challenges and opportunities of social media, _Business horizons_ 53(1), 59–68. 
<sup>7</sup> Chui, M., Manyika, J., Bughin, J., Dobbs, R., Roxburgh, C., Sarrazin, H., Sands, G. and Westergren, M.: 2012, The social economy: Unlocking value and productivity through social technologies. [https://www.mckinsey.com/industries/high-tech/our-insights/ the-social-economy](https://www.mckinsey.com/industries/high-tech/our-insights/ the-social-economy) [Accessed 18 May 2019]. 
<sup>8</sup> Edosomwan, S., Prakasan, S. K., Kouame, D., Watson, J. and Seymour, T.: 2011, The history of social media and its impact on business, _Journal of Applied Management and entrepreneurship_ 16(3), 79–91.
<sup>9</sup> He, W., Shen, J., Tian, X., Li, Y., Akula, V., Yan, G. and Tao, R.: 2015, Gaining competitive intelligence from social media data: evidence from two largest retail chains in the world, _Industrial Management & Data Systems_ 115(9), 1622–1636.
<sup>10</sup> Brooker, P., Barnett, J., Cribbin, T. and Sharma, S.: 2016, Have we even solved the first ‘big data challenge?’practical issues concerning data collection and visual representation for social media analytics, _Digital methods for social science_, Springer, pp. 34–50.
<sup>11</sup> Mayeh, M., Scheepers, R. and Valos, M.: 2012, Understanding the role of social media monitor- ing in generating external intelligence, ACIS 2012: Location, location, location: _Proceedings of the 23rd Australasian Conference on Information Systems 2012_, ACIS, pp. 1–10. 
<sup>12</sup> Halasz, C. M.: 2019, Optimizing training for sparse workloads in Tensorflow. Reinforce AI Conference. **URL**: [https://reinforceconf.com/speaker/CibeleMontezHalasz](https://reinforceconf.com/speaker/CibeleMontezHalasz)
<sup>13</sup> Dou, W., Wang, X., Skau, D., Ribarsky, W. and Zhou, M. X.: 2012, Leadline: Interactive visual analysis of text data through event identification and exploration, _2012 IEEE Conference on Visual Analytics Science and Technology (VAST)_, IEEE, pp. 93–102.
<sup>14</sup> Hogan, B.: 2016, Social media giveth, social media taketh away: Facebook, friendships, and apis, _International Journal of Communication_, Forthcoming. 
<sup>15</sup> Weller, K. and Kinder-Kurlanda, K. E.: 2015, Uncovering the challenges in collection, sharing and documentation: The hidden data of social media research?, _Ninth International AAAI Conference on Web and Social Media_.

---

[.text: alignment(left)]

# References

<sup>16</sup> Altshuler, Y., Pan, W. and Pentland, A. S.: 2012, Trends prediction using social diffusion models, International Conference on Social Computing, _Behavioral-Cultural Modeling and Prediction_, Springer, pp. 97–104.
<sup>17</sup> Sapountzi, A. and Psannis, K. E.: 2018, Social networking data analysis tools & challenges, _Future Generation Computer Systems_ 86, 893–913.
<sup>18</sup> Figueiredo, F., Almeida, J. M., Gon ̧calves, M. A. and Benevenuto, F.: 2016, Trendlearner: Early prediction of popularity trends of user generated content, _Information Sciences_ 349, 172–187. 
<sup>19</sup> Qian, S., Zhang, T., Xu, C. and Shao, J.: 2015, Multi-modal event topic model for social event analysis, _IEEE transactions on multimedia 18(2)_, 233–246.
<sup>20</sup> Manovich, L.: 2011, Trending: The promises and the challenges of big social data, _Debates in the digital humanities_ 2, 460–475. 
<sup>21</sup> Schroeder, R.: 2014, Big data and the brave new world of social media research, _Big Data & 
Society_ 1(2).
<sup>22</sup> Sloan, L. and Quan-Haase, A.: 2017, The SAGE handbook of social media research methods, 
Sage.
<sup>23</sup> Adar, E. and Adamic, L. A.: 2005, Tracking information epidemics in blogspace, Proceedings of the 2005 IEEE/WIC/ACM international conference on web intelligence, _IEEE Computer Society_, pp. 207–214.
<sup>24</sup> Gomez-Rodriguez, M., Leskovec, J. and Krause, A.: 2012, Inferring networks of diffusion and influence, _ACM Transactions on Knowledge Discovery from Data_ (TKDD) 5(4).
<sup>25</sup> Cannarella, J. and Spechler, J. A.: 2014, Epidemiological modeling of online social network dynamics, _arXiv preprint arXiv:1401.4208_.
<sup>26</sup> Chang, H.-C.: 2010, A new perspective on twitter hashtag use: Diffusion of innovation theory, _Proceedings of the American Society for Information Science and Technology_ 47(1), 1–4.
<sup>27</sup> Jamieson, J. and Boase, J.: 2017, Listening to social rhythms: Exploring logged interactional data through sonification, _The SAGE Handbook of Social Media Research Methods_.
<sup>28</sup> Liu, F., Wang, L., Johnson, H. and Zhao, H.: 2015, Analysis of network trust dynamics based on the evolutionary game, Scientia Iranica. Transaction E, _Industrial Engineering_ 22(6). 
<sup>29</sup> Schmidt, C. W.: 2012, Trending now: using social media to predict and track disease outbreaks.
<sup>30</sup> Zimmer, M. and Proferes, N. J.: 2014, A topology of twitter research: disciplines, methods, and ethics, _ASLIB Journal of Information Management_ 66(3), 250–261.

---

[.background-color: #ff0000]
References

---

# [fit] Insights into **Social Media** Data: 
# [fit] a new formalism inspired in **Thermodynamics**

![](assets/thermo.jpg)

![inline 140%](assets/qr.jpg)

All images are CC0, Pixabay-licensed or my own
See **github.com/TheMartianLife/Honours-Presentation**


