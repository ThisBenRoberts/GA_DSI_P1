# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Overview

We're going to take a look at aggregate SAT and ACT scores and participation rates in the United States. We'll seek to identify trends in the data to address our problem statement.

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

---
### Problem Statement

We hypothesize that ACT/SAT test scores, in composite, can be used as an indicator for the effectiveness of educations across the United States. This project seeks to determine if a relationship exists between particpation and outcomes of the SAT/ACT to support or oppose the continuation of these tests as a benchmark for the effectiveness of state education programs.


---
### Datasets

#### Provided Data

We were provided with 6 datasets that were used in this analysis. These datasets were 

* [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State ([source](https://blog.prepscholar.com/average-sat-scores-by-state-most-recent))

#### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT Combined| State in which the exam were given
|act_participation_17|float|ACT/SAT Combined|% of student who too the ACT in 2017
|act_composite_17|float|ACT/SAT Combined|Average score for ACT exams administered in 2017
|act_participation_18|float|ACT/SAT Combined|% of student who too the ACT in 2018
|act_composite_18|float|ACT/SAT Combined|Average score for ACT exams administered in 2018
|act_participation_19|float|ACT/SAT Combined|% of student who too the ACT in 2019
|act_composite_19|float|ACT/SAT Combined|Average score for ACT exams administered in 2019
|sat_participation_17|float|ACT/SAT Combined|% of student who too the SAT in 2017
|sat_total_17|float|ACT/SAT Combined|Average score for SAT exams administered in 2017
|sat_participation_18|float|ACT/SAT Combined|% of student who too the SAT in 2018
|sat_total_18|int|ACT/SAT Combined|Average score for SAT exams administered in 2018
|sat_participation_19|float|ACT/SAT Combined|% of student who too the SAT in 2019
|sat_total_19|float|ACT/SAT Combined|Average score for SAT exams administered in 2019
---

### Analysis Summary

For this analysis, the average ACT Scores, and SAT Scores, for 2017, 2018, and 2019, as reported at the state level, were examined. The data included state names, measures of participation, and, in some cases, average scores broken down by section. English, Mathematics, Reading, and Science for the ACT. Evidence-Based Reading and Writing and Math for the SAT.  Since the scores per section were not available in all years, the composite or total scores were used.  Those scores were compared to the states level of participation in order to determine if there was correlation, either positive or negative to the overall average score with the goal of helping us determine if a state's overall SAT or ACT score can be used as a fair baramoter of the effectiveness of the state's education program in relation to other states.

---

### Conclusions & Recommendations

There is indeed a correlation between participation in the ACT / SAT Exams and the stat'es average or composite scores.  While the trend appears to be stronger for the ACT, for both exams the lower the level of participation, the higher the average score per state.  Knowing that some states require the ACT or SAT exam in order to graduate high school, in these states it is reasonable to assume that students with little desire or no intention of attending college are taking the exam along side student who have prepped for years to take these exams.  In those states, with 100% participation, the average ACT / SAT score could be used to compare education programs from state to state and to monitor imporvement from year to year so long as the requirement remains in effect.  

Conversly, we suspect that in states with lower levels of particpiation, those taking the ACT or SAT desire or intend to go on to higher levels of education and have prepped accordingly.  Meaning the test taking populations in those states are by default more likely to score higher on the exams.  With fewer unprepared test takers in the population, the average score across these states remains high. As a result, we would not reccomend using the average ACT / SAT score to compare education programs from state to state or to monitor improvement from year to year.  
