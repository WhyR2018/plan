# Constructing scales from survey questions

[Tomasz	Żółtak,	Educational Research Institute (Warsaw, Poland)]()

## Description

Surveys often include sets of questions on the same subject, designed to create more general indicators of views, attitudes, knowledge or other characteristics of respondents. Such an indicators allow for synthesis of information, drawing more general conclusions and reduction of random measurement errors. As continuous variables, they are also easier to use in further analysis.

However, the use of survey questions often involves a number of problems:
- answers are given on scales that can’t be treated as continuous (eg. a Likert scale);
- response to the questions may depend on the way in which they are worded, eg. respondents may react a little different to negative statements;
- respondents may have different styles of answering questions, eg. some may prefer more extreme answers than the other;
- in self-assessment questionnaires some respondents may be inclined to give untruthfully answers indicating a higher level of knowledge or skills.

Workshop participants will learn how to use R to:
- create scales based on sets of categorical variables using Categorical Exploratory/Confirmatory Factor Analysis (CEFA / CCFA) and IRT models;
- use models with bi-factor rotation to deal with different forms of asking questions;
- correct for differences in a style of answering questions asked using a Likert scale;
- use the possibility to correct self-assessment knowledge/skill indicators using fake items.

During the workshop R packages ‘polycor’, ‘mirt’ and ‘laavan’ will be used along with the data from international surveys: ESS, PISA and PIAAC.