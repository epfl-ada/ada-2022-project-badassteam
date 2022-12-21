---
layout: default
---
![image](/output/Intro.jpg)

# Introduction

In 1975, the filmmaker Laura Muley highlighted the underrepresentation of women in film industry and more broadly in visual culture. She introduced the term "male gaze" and allow people to question the place of women in the cinema industry. The American cinema industry played a strong role on the western society and appears as a good area of study to examine how women's representation has changed over the period of nearly a century.

This datastory begins with a trio of datasets from the <strong>CMU Movie Summary Corpus</strong>: the first dataset includes information on 81741 movies from 1915 to 2012, the second dataset features information on the characters who appeared in these movies, and the final dataset includes summaries of the movies in the first dataset

The central focus of this project is to thoroughly analyze movie summaries, which hold a vast amount of information about the films. In addition to examining the <strong>main character</strong> and other key details, we will also delve into the representation of <strong>male and female actors in the movies</strong>. Through the analysis of summaries, we can gain a deeper understanding of the roles and portrayal of male and female characters in the film industry, as well as any potential biases or trends in the depiction of these characters.


How has the women places evolves in the US cinema industry ? Does the cinema represent more men than women and has there been a change over the years ? Has the role played by woman and the attributes of their characters evolves through the year ? And finally how the place of actresses evolve for the public ?

Given all of these factors, several questions come to mind:

* Is it possible to define the main character from a summary ?
* Does the genre of the movie impacts how women are represented ?
* 

## Project pipeline

## The world of cinema through American eyes ?

Thanks to a preliminary study, it has been chosen to focus on American movies in the global cinema industry. This focus is appropriate for this case because Hollywood has produced half of the movies made worldwide and has the largest pool of acting talent.

Country                      |	code |	Number_of_movie |	Percent | Number of act | Male acting | Female acting |
|:---------------------------|:------|:-----------------|:----------|:--------------|:------------|:--------------|	
['United States of America'] |	USA	 | 34408	        | 39.806106	| 226169        | 152713      | 73456         |
['India']                    |	IND  |	8411	        | 9.730561  | 45729         | 30024       | 15705         |	
['United Kingdom']           |	GBR  |	7868	        | 9.102373  | 48592         | 32837       | 16183         |
['France']                   |	FRA	 | 4395	            | 5.084510  | 25429         | 16183       | 9246          |	
['Italy']                    |	ITA	 | 3163	            | 3.659228	| 14750         | 9740        | 5010          |
...                          |	...	 | ...	            | ...	    | ...           | ...         | ...           |
['Republic of China']        |	CHN	 | 1	            | 0.001157  | 3             | 2           | 1             |
['Macau']                    |	MAC	 | 1	            | 0.001157	| 3             | 1           | 2             |
['Palestinian Territories']  |	PSE	 | 1	            | 0.001157	| 0             | 0           | 0             |


{% include world_map.html %}


![image](/output/MovieByDecade.png){:style="display:block; margin-left:auto; margin-right:auto"}



![image](/output/GenreByDecade.png){:style="display:block; margin-left:auto; margin-right:auto"}

## What can a director's point of view reveal in a summary ?

The study aims to examine the evolution of female characters as depicted by movie directors. One way to do this is by analyzing summaries of films, as they often contain information about characters and their attributes. This can provide insight into how women have been portrayed and represented in films over time, and how this has changed or evolved. It is important to approach this analysis objectively and consider multiple perspectives, rather than relying on personal opinions or biases.

### how to extract character from summary
To begin we extract all the characters from summaries thanks to a Machine Learning algorithm which leaks all pronoms to their related name. With this, we found a list of character by movie. We rank them and find the main character. 

{% include Charac_ranking.html %}
### repartion of character per decade
{% include Charac_decade.html %}
### repartition of character per genre
{% include Genre_decade.html %}


## Analysis diference man woman thks to summary

![image](/output/MF_Adjective_decade.png){:style="display:block; margin-left:auto; margin-right:auto"}
![image](/output/MF_Verb_decade.png){:style="display:block; margin-left:auto; margin-right:auto"}

![image](/output/Adj_frequency.png){:style="display:block; margin-left:auto; margin-right:auto"}


## Comparison to public sentiment 
## Use grade on each movie

## Conclusion




