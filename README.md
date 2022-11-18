# ada-2022-project-badassteam

Created by:\
Antoine LAPERRIERE - 288734\
Benoit GAUDIOT - XXXXXX\
Nathan PAILLOU - XXXXXX\
Romain BEZEAUD - 283622


# Actresses and Cinema, a representation of our society?

 ___Study of the evolution of the woman place in the US cinema industry from 1888 to 2012___

## Abstract

Hollywood, the biggest cinema industry in the world. As the women places is increasing through the year, it is 

## Research questions

* How has the women places evolves in the US cinema industry ? Has the role they played evolves through the year ? Has the attributes of the characters they played change ? 

## Proposed additional datasets
### Wikidata


* **Freebase_ID <=> Q-wikidata ID**: The first step was to find the correspondance between the freebase_ID that we have in our dataset with the Q-ID wikidata uses to classify the pages.
For this, a SPARQL query has been made to extract all the movies that were made in the US and that has a freebase_ID. This query allows us to obtain a table with a row containing the freebase_ID and the other row with the corresponding Q-ID.

* **Review score**: The next step was to add the review score to our dataset. For this, we search for the US movies that has a freebase_ID and a review score. Then, we also query the website from which the score was coming and the type of review. With the obtained data, we chose to keep two differents review score both from [Rotten Tomatoes](https://www.rottentomatoes.com): the tomatometer score and the average review score. The first one is based on press reviews (À VÉRIFIER) whereas the second is based on the website users. These indicators could be interesting to observe if the popularity of a film could be linked to the cast.



## Methods

**Step 1: Data scraping, pre-processing and dataset construction.**

* Dataset D1 : General dataset containing movies between 1888 and 2012
* Dataset D2 : Character dataset with role from movies of dataset D1
  * D2.1 : Subsets by gender of speaker
  * *These subsets are built later on during Step 4.*
* Dataset D3 : 
  * D3.1: 

**Step 2: General preliminary analysis on movies, actors and actresses around the world**
Analyse the numbers of movies turn in differents countries of the world. Also looks on numbers of role played by actors and actresses. 

**Step 3: Generate annual word clouds based on dataset D1 with this [library.](https://github.com/amueller/word_cloud)**

**Step 4: Investigate gender, political and generational biases in MeToo coverage using NLP to answer question A).**
Train a [SpaCy NLP model](https://spacy.io/usage/training) with dataset AD3 to perform sentiment analysis. Classification thanks to trained model on the whole dataset D2. Subdivision of D2 into D2.1, D2.2 and D2.3 for biases investigation. Clustering trials with unsupervised different ML algorithms applied on the sentiment analysis classification probabilities.

**Step 5: Investigate general women perception via dataset D3 in medias to answer question B).**
Generate word clouds. Classification of quotes : Text Blob or Vader models for positive, negative or neutral. Train SpaCy model on AD2 for misogynistic or non misogynistic. Classification thanks to trained model on D3.

**Step 6: Correlate and investigate causation between MeToo general perception and women’s mediatic place to answer question C).**
Plot previously collected (step 5) data distributions according to time. Comparison with key turning points of MeToo. Investigation of the statistical significance of detected changes before and after MeToo.

**Step 7: Github site building and Datastory redaction.**

**Further details on the proposed data pipelines can be found in the notebook.**

## Proposed timeline
* 
* **02.12.22 homework 2 deadline**
* 16.12.22 : complete code
* 20.12.22 : complete datastory
* **23.12.22 : Milestone 3 deadline**

## Organization within the team

* Antoine :
* Benoit :
* Nathan :
* Benoit :
