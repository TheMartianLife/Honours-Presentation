theme: Next, 1
autoscale: true
slidenumbers: true
slidecount:true
header-strong: #FFFFFF
footer: A BICT Honours project by Mars Geldard, under the supervision of Professor Paulo de Souza and Dr James Montgomery (2019).

[.slidenumbers: false]
[.hide-footer]

# [fit] Insights into **Social Media** Data: 
# [fit] a new formalism inspired in **Thermodynamics**

![](assets/thermo.jpg)

---

# Overview

A new proposed method for **trend analysis and prediction** with **social media** data that was inspired by the theory of **entropy** from thermodynamics as it has grown and been applied to other fields.

Quantitative exploratory study (in three parts) involves calculating **entropy over time** in pre-existing **Twitter** datasets, looking for **two predicted behaviours** as key indicators of feasibility.

---

[.slidenumbers: false]
[.hide-footer]

# **Background**

![](assets/books.jpg)

^ Provides a clear and comprehensive review and critical appraisal of key literature relevant to the proposed research.

^ Significance of the research is contextualised within the literature presented.

---

[.slidenumbers: false]
[.hide-footer]

# Social Media

![](assets/social.jpg)

---

[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: impact of social media

---

[.slidenumbers: false]
[.hide-footer]

# Social Media Analysis

![](assets/insights.jpg)

---

[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: motivators and challenges in social media analysis

---

[.slidenumbers: false]
[.footer: Cibele Montez Halasz, Senior ML Engineer from Twitter, speaking at Reinforce Conf (Budapest, 2019)]

![](assets/reinforce.jpg)

---

[.slidenumbers: false]
[.hide-footer]

# Trend Analysis & Prediction

![](assets/stocks.jpg)

---

[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: motivators and challenges in social media trend analysis

---

# Challenges

* Timeliness of analysis and detection
* Privacy concerns
* False positives in anomaly detection methods
* Reliance on other information sources in alternative methods
* Predicting the future? 🤔

---

# Multidisciplinary challenges

* Very human data; erratic behaviours (**behavioural science**)
* Sharing between non-fully-connected graph structure... (**graph theory**)
* ...of nodes with varying levels of transmissiveness (**information diffusion**)
* Different content and sentiments get shared in different ways (**social contagion**)

---

[.slidenumbers: false]
[.hide-footer]

# Analogous Application

![](assets/curve.jpg)

---

[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: analogous applications of methods from other fields

---

# The Gist

* Social Media use has swept across the globe, impacting the way we communicate, conduct business and view society

* Analysing behaviour on Social Media is seen as important to understanding the opportunities and risks it presents

* Where current methods targeting Social Media have been lacking, a small group of studies have shown varying success in applying methods of analysis from other fields

---

[.slidenumbers: false]
[.hide-footer]

# Entropy Theory

![](assets/space.jpg)

---

[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: some have proposed entropy theory, but only in Information Theory form (and still no-one seems to have done it)

---

[.slidenumbers: false]
[.footer: [3] Tsou (2015)]

![](assets/entropy1.png)

---

[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: why its nearer-to-thermodynamics form may be more suitable

---

[.slidenumbers: false]
[.text: #000000]
[.footer: [1] Mahbub, de Souza and Williams (2016)]

![](assets/proposal.png)

---

## Boltzmann's Entropy

$$
S=k \ln (N)
$$
<br><br><br>

```python
# python equivalent (simplified)
def boltzmann(s):	
    k = scipy.constants.Boltzmann
    n = len(s.possible_microstates)
    return k * math.log(n)
```

---

## Gibb's Entropy

$$
S=-k \sum_{i} P_{i} \ln P_{i}
$$

```python
# python equivalent (simplified)
def gibbs(s):
    k = scipy.constants.Boltzmann
    entropy = 0
    for i in set(s):
        p_i = s.count(i) / len(s.possible_microstates)
        entropy += p_i * math.log(p_i)
    return -k * entropy
```

---

## Shannon's Entropy

$$
S=-\sum_{i} P_{i} \ln P_{i}
$$

```python
# python equivalent (simplified)
def shannon(s):
    entropy = 0
    for i in set(s):
        p_i = s.count(i) / len(s.possible_microstates)
        entropy += p_i * math.log(p_i)
    return -entropy
```

---

# Entropy over time

* Reveals descriptive statistical measures about a set of data
* But also measures diversity and internal inconsistency
* Takes focus away from upper and lower bounds—or even ranges—in favour of changes in internal distribution that may be more informative
* Is in some cases sufficient to adapt analysis into Markov-model-based prediction

---

[.slidenumbers: false]
[.hide-footer]

# **Aims & Objectives**

![](assets/target.jpg)

^ Aims and objectives are concisely elaborated.

^ Original and highly relevant hypotheses or research questions are clearly articulated (if appropriate).

---

# Broadly

1. Can the analogous application of **Entropy Theory** present useful information about the lifetime of a trend or topic on a Social Media platform?
2. Is there indication that the method could be applied more broadly, or adapted to be **predictive**?

---

# In this study

Experimentation aims to confirm the dual hypotheses as follows:

1. **increasing entropy over time** may suggest impending critical interest preceding a trend developing to significance, and
2. **decreasing rate of entropy increase over time** after a high entropy or engagement level has occurred may suggest new evolution in the topic.

---

# In further investigation

If we can predict changes in topic growth over time, this may aid in early detection of trends. 

This may allow researchers better comparative investigation into factors that affect trends on social media, or other parties the ability to leverage such predictions.

---

# In further investigation

Additionally, if we can extrapolate from individual topics the _enthalpy_ (potential energy/engagement/interest) of the overall platform, then we can

* map whether and how this fluctuates,

* get an idea of how much of it is being used at any given time and by which topic areas, and

* analyse which topic areas require/hold/generate the most energy.

---

# Potential **commercial** value

Assuming we can look at the platform and get an idea of

1. the total energy potential right now, 

2. the total energy being used by different topics right now, and

3. the total energy required, held and/or generated by different topics overall

then information release could be optimised for times when potential energy in their topic area is being under-utilised.

---

# Potential **social research** value

Assuming we can predict trend decay over time if no new stimulus is received, we can identify points where new external stimulus probably was received, even where it is not evident in the platform content.

This can help identify new context or anomalous trends.

---

[.slidenumbers: false]
[.hide-footer]

# **Research Design**

![](assets/research.jpg)

^ Presents a clear, comprehensive and appropriate methodology for the research including research philosophy, research strategy and research design.

^ Research design details the approach, the tools and techniques for data collection, collation, analysis, discussion and interpretation (where appropriate) of the research data.

---

# Two main steps:

## 1. Creating data
## 2. Analysing data

---

[.slidenumbers: false]
[.hide-footer]

![](assets/harvest.jpg)

# Harvesting from Twitter

---

# Why Twitter?

* Rapid generation of content, rapid decline in interest => easily observable trends
* Discrete content size easier to analyse => more easily verifiable datasets
* Reasonable breadth of functionality in API, well-established tools for research => easier to perform and recreate studies

---

# Twitter Content

* Posts of maximum 140 characters (**tweets**)
* Accompanying media of one video or up to four images
* May include hashtags, stock tickers, tagged users
* Metadata includes time of posting, engagements, location
* Sharing posts can be done verbatim (**retweets**) or with added commentary (**quote tweets**)

---

[.slidenumbers: false]
[.hide-footer]

![](assets/datasets1.png)

---

[.slidenumbers: false]
[.hide-footer]

![](assets/datasets2.png)

---

# Datasets needed for this study

1. Representing a **single** cohesive topic growing over time
2. Representing a higher-level topic with **multiple** sub-topics or evolution over time

---

[.slidenumbers: false]
[.hide-footer]

![](assets/set1.png)

---

[.slidenumbers: false]
[.hide-footer]

![](assets/set2.png)

---

[.slidenumbers: false]
[.hide-footer]

![](assets/twarc.png)

---


[.background-color: #FF0000]
[.text: #000000]

Summarise lit review: studies that use Twarc

---

[.slidenumbers: false]
[.hide-footer]

![](assets/docnow.png)

---

[.slidenumbers: false]
[.hide-footer]

![](assets/split-files3.jpg)

---

[.slidenumbers: false]
[.hide-footer]

```python
# split.py (simplified)

# create generator function for input file of tweet IDs
def splitter(file, n):
	lines = list(file)
	for i in xrange(0, len(lines), n):
		yield lines[i: i + n]

with open(INPUT_FILENAME,'r') as input_file:
	
	# partition file by given size
	for index, lines in enumerate(splitter(input_file, BATCH_SIZE)):
		batch_filename = OUTPUT_FILENAME + str(index) + '.txt'

		# write each batch to new file
		with open(batch_filename, 'w+') as output_file:
			output_file.write('\n'.join(lines))
```
---

![fit](assets/split-files.png)

---

![fit](assets/split-files2.png)

---

[.slidenumbers: false]
[.hide-footer]

```python
# hydrate.py (simplified)
import json, twarc

# create generator function for input file of tweet IDs
def tweet_ids():
    for id in open(INPUT_FILENAME):
        yield id

# setup Twarc with API key credentials from created Twitter Developer account
twarc = twarc.Twarc(key, secret, token, token_secret)

# fetch JSON values as dictionary from API with use of hydrate() function
tweets_dict = { 'tweets': [] }
for tweet in twarc.hydrate(tweet_ids):
	tweets_dict['tweets'].append(tweet)

# convert to JSON and write to output file, one line per tweet
with open(OUTPUT_FILENAME,'w+') as output_file:
    json.dump(tweets_dict, output_file)
	
```	
---

# Tweet JSON

```json
{
   "created_at":"Fri Feb 10 10:05:45 +0000 2017",
   "id_str":"8299945678410624",
   "full_text": "This is a fake Tweet because I like to err on the side of privacy.",
   "user":{
      "id_str": "972937630",
      "name": "John Doe",
      "screen_name": "johndoe",
      "protected": false,
      "verified": false,
   },
   "retweet_count": 167,
   "favorite_count": 50
}
```

---

| File | IDs | Hydrated | Lost |
|:---:|:---:|:---:|:---:|
| immigration-exec-order1 | 500,000 | 342,551 | 157,449 |
| immigration-exec-order2 | 500,000 | 341,873 | 158,127 |
| immigration-exec-order3 | 500,000 | 344,425 | 155,575 |
| immigration-exec-order4 | 500,000 | 375,875 | 124,125 |
| immigration-exec-order5 | 500,000 | 364,173 | 135,827 |
| immigration-exec-order6 | 500,000 | 364,605 | 135,395 |
| immigration-exec-order7 | 500,000 | 332,024 | 167,976 |
| ... | ... | ... | ... | 
| **Total** | 16,875,766 | 11,776,307 | 5,099,459 |

---

## seemingly random yet consistent distribution of missing datapoints
## = 
## suitably random self-selecting population sample 👍

---


[.slidenumbers: false]
[.hide-footer]

```python
# tweets.py (simplified)
import csv, jsonl
from classes import Tweet

headers = ['id', 'likes', 'retweets', 
	'retweeted_id', 'quoted_id', 'timestamp']

with open(INPUT_FILENAME, 'r') as input_file:
	output_file = open(OUTPUT_FILENAME,'w+')
	csv_writer = csv.writer(output_file, delimiter=',')
	csv_writer.writerow(headers)

	for line in input_file:
		tweet = Tweet(line)
		csv_writer.writerow(tweet.values())
	output_file.close()
```

---

![100%](assets/beachball.png)

---

[.slidenumbers: false]
[.hide-footer]

```python
# classes.py (simplified)
import json

class Tweet():

	def __init__(self, tweet_object):
        	tweet_json = json.loads(tweet_object)

        	self.id = int(tweet_json["id_str"])
        	self.likes = int(tweet_json["favorite_count"])
        	self.retweets = int(tweet_json["retweet_count"])
        	self.timestamp = self.process_datetime(tweet_json["created_at"])

        	# RETWEET
        	if "retweeted_status" in tweet_json:
            		self.retweeted_id = int(tweet_json["retweeted_status"]["id_str"])
            		self.likes = int(tweet_json["retweeted_status"]["favorite_count"])

        	# QUOTE TWEET
        	if "quoted_status" in tweet_json:
            		self.quoted_id = int(tweet_json["quoted_status_id"])
```

---

# Phase 1: Exploration

* Establish "ground truth" of trend behaviour over time portrayed in each dataset 
* Decide on appropriate granularity for discretisation of data (or justify use of full range of values)
* Explore descriptive statistics to establish theoretical bounds
* Develop strategies for dealing with missing data and edge cases

---

# ⚠️ Issues

1. Retweeted tweets show no information about whether likes were given to original or retweet
2. Engagement metrics are associated with time of posting, even though they would have occurred later and over time

It is assumed that the presence of both effects in **both the test and comparison data** will nullify the effect. 

*But* this study can only assert indicative suitability for historical data until verified with a live study.

---

[.slidenumbers: false]
[.hide-footer]

![](assets/piles.jpg)

---

[.slidenumbers: false]
[.hide-footer]

```python
# collate.py (simplified)
with open(INPUT_FILENAME, "r") as input_file:
	csv_reader = csv.reader(input_file, delimiter=',')
	output_files = {}

	for line_number, line in enumerate(csv_reader):
		date = line[5][0:10] # YYYY-MM-DD

		if date not in output_files:
			new_filename = OUTPUT_FILENAME + "-" + date + ".csv"
			output_files[date] = open(new_filename,"a+")

		output_file = output_files[date]
		output_file.write(",".join(line) + '\n')

for file_handle in output_files.keys():
	file_handle.close()
```
---

![fit](assets/dated.png)

---

[.slidenumbers: false]
[.hide-footer]

```python
# entropy.py (simplified example)
import csv, bumpy

output_file = open(OUTPUT_FILENAME, 'w+')
csv_writer = csv.writer(output_file, delimiter=',')
cumulative_likes = 0
likes = []

for input_filename in INPUT_FILENAMES:
	input_file = open(input_filename, 'r')
	csv_reader = csv.reader(input_file, delimiter=',')

	likes += [float(row[1]) for row in csv_reader]
	date = input_filename[23:33] # YYYY-MM-DD
	cumulative_likes += numpy.sum(likes)
	csv_writer.writerow([date, str(entropy(likes)), str(cumulative_likes)])

	input_file.close()

output_file.close()
```

---

# [fit] Phase 2: Cohesive topic
# &
# [fit] Phase 3: Evolving topic

---

[.slidenumbers: false]
[.hide-footer]

![](assets/response.jpg)

## Inferential analysis = 
## dynamic + reponsive

---

## Predictions

# ![160% inline](assets/loglinear.png)

* Normal-ish distribution of new tweets
* Varying loglinear to exponential growth rates in engagement
* Engagements between 0 and ~500,000

---

### The Kolmogorov-Smirnov & Cucconi Tests

# ![200% inline](assets/kolmogorov.png)

---

### Regression analysis

# ![78% inline](assets/regression.png)

---

[.slidenumbers: false]
[.hide-footer]

## Scaling + Transforming

![](assets/scale.jpg)

---

[.slidenumbers: false]
[.hide-footer]

## Data Segmentation

![](assets/segment.jpg)

---

[.slidenumbers: false]
[.hide-footer]

![](assets/base-jump.jpg)

---

# Preliminary Findings
#### (_very_ preliminary, I only just managed to hydrate a complete dataset on Sunday)

---

[.background-color: #FFFFFF]
[.text: #000000]

![170%](assets/preliminary.png)

---

# Revisiting hypotheses

I theorised that the patterns to emerge would be two-fold:

1. **increasing** entropy over time **preceding a trend** developing to significance, and
2. **decreasing** rate of entropy increase over time after a high entropy or engagement level **preceding changes in behaviour**.

---

[.background-color: #FFFFFF]
[.text: #000000]

![170%](assets/preliminary2.png)

---

# ...maybe that was too easy? 🤔

---

# References

1. Mahbub, M.S., de Souza, P. and Williams, R., 2017. Describing environmental phenomena variation using entropy theory. _International Journal of Data Science and Analytics_, 3(1), pp.49-60.
2. Mahbub, M.S., de Souza, P. and Williams, R., 2019. Understanding Environmental Changes Using Statistical Mechanics. _Annals of Data Science_, pp.1-13.
3. Tsou, M.H., 2015. Research challenges and opportunities in mapping social media and Big Data. _Cartography and Geographic Information Science_, 42(sup1), pp.70-74.

---

[.slidenumbers: false]
[.hide-footer]

# [fit] Thank you!

![](assets/fireworks.jpg)

* All images are CC0, Pixabay-licensed or my own
* See **github.com/TheMartianLife/Honours-Presentation**

![inline 112%](assets/qr.jpg)

---

[.background-color: #FF0000]
[.text: #000000]
[.header: #000000]

### more slides will go here with visualisations of answers to questions that friends ask me when rehearsing
### (that I can't justify or fit in the main presentation)
