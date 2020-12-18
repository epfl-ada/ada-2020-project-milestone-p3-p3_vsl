# P3 milestone : proposition of paper extension 


## Study of the existence of differences in the police stop schemes among police officers in the US

## Abstract

Using various methods trying to remove potential biases (veil of darkness, threshold test…), the original paper studies the overall racial bias in the police stops across the US. As an extension, we propose a more detailed analysis of this bias among the police forces. In particular, the study of how the characteristics of a police officer (race, gender, age, experience) influence this bias. This could shed light on more concrete social issues : for instance, finding that the time of service increases the degree of bias of an officer could show, under careful assumptions, that the very fact of working among the police enhances the bias. Solution could be to re-think the typical policer career plan to try to limit this effect. Following the recent events involving police in the US, we may wonder if this bias has evolved during the last few years, and how. We will thus study if one could spot a difference in the stop biases between now and 10 years ago.

## Research questions

1. In which way does the characteristics (race, genre, experience, age) of the officers influence the race of the subjects that they tend to arrest ? 
   - Can we draw characteristics of the officers more involved in arrest of Black, Hispanic and White drivers ?
   - Are there obvious biases ? (e.g black officers tend to arrest more white drivers / white officers tend to arrest more black drivers / experience officer tend to be less/more biased)
2. More particularly, does the time spent in the police forces influence the racial bias of officers ? 

3. Once stopped, does the characteristics of the officer influence the search ? In particular, is it prejudiced against minorities ? 
<!-- 4. (if time) Is there an influence of the epoch on these results? (e.g 2008 vs. 2018) -->


## Proposed datasets

The original paper based its work on a tremendous amount of data available on the website https://openpolicing.stanford.edu/data . As lots of features were not explored in the paper, we decided to use the same bulk. Among all the datasets, we sorted out the ones referencing the characteristics of the officer carrying out the arrest, as well as a sufficient time lapse. Given the characteristics of the officer and the details about the arrest we are interested in, the dataset we are going to use is composed of the arrests conducted by the **state police of Florida**, as well as the municipal police of **Long beach, California**.

## Methods

- To analyse the influence of the officer’s features on its racial bias : (NB: we want to compare the officers here, the probable existence of a bias in stops was established by the paper)
  - Define a “bias score” for each officer (e.g : proportion of minority they arrested overall their career) 
  - Use a linear regression analysis f(officer_features) = bias_score to analyse the weight of the various features of the officer
- To study of the differences in arrest according to the race of police officer
  - Possible to simply compare the distributions in the 3 main categories
- To analyse the influence of the years spent in police forces 
  - Option 1 : study the evolution in the bias score of the officers that stayed more than Y years 
  - Option 2 : Compare officers that spent less N years in the police with more than M years
- Influence of epoch
  - Same analysis but old vs. recent time periods 


## Proposed timeline

| Step | Explanation | Due date |
|----------|:-------------:|------:|
| Preparation of dataset | Collecting all data from LongBeach and FL. Selecting relevant features. | 4/12 |
| Definition of bias score | Find the best available way to measure bias with our tools. Evaluate possible bias in our results and find way to overcome them. | 9/12 |
| Study of officer characteristics | Use data with regressions and comparison to find influences / or not, of the characteristics of the police officers | 15/12 |
| Study of temporal effect | Repeat the same study but with subsets of all data (old data and more recent data) to see potential evolution of bias through tme| 16/12 |
| Report redaction | Write latex report / paper about conclusions. Draw conclusions and evalutate the potential bias of our results. | 18/12 |
||||


## Organization within the team

Mickael : first insight of the data, first idea of bias score and raw analysis

Samuel : handle plotly and transfer plt to interactive graphs. Second idea of bias score

Mickael & Samuel : search_rate graphs

Jonas : thinking and implementation of Veil of Darkness

Power of friendship : everyone wrote the datastory

