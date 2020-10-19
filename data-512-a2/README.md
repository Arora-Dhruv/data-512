
# Human Centered Data Science - A2 Bias in Data

The project analyze the Wikipedia Talk corpus which is being used to train machine learning models as part of a project called [Conversation AI](https://conversationai.github.io/)  by Google data scientists. The purpose of the analysis is to identify what, if any, sources of bias may exist in these datasets, and to develop testable hypotheses about how these biases might impact the behavior of machine learning models trained on the data, when those models are used for research purposes or to power data-driven applications.  
The <a id="https://meta.wikimedia.org/wiki/Research:Detox/Data_Release">Wikipedia talk corpus </a> consists of three datasets. Each dataset contains thousands of online discussion posts made by Wikipedia editors who were discussing how to write and edit Wikipedia articles. Crowdworkers labelled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”. Many posts in each dataset were labelled by multiple crowdworkers for each type of hostile speech, to improve accuracy.  
  
We have used two of three of the hostile speech: toxicity & aggression for the analysis. 

## Research questions for this study are:  
* How consistent are labelling behaviours for <b> toxicity</b> hostile speech among workers with different demographic profiles?  
* Are certain words more likely to be associated with comments labelled as hostile speech - toxicity vs aggression?

Both the research questions are intended to find potential bias in data if exists and further discuss the implications of bias found.

## Data Source
I have used two of the three hostile speech data for performing analysis on above research questions:
1. [Toxicity Datasets](https://figshare.com/articles/Wikipedia_Talk_Labels_Toxicity/4563973) Version 2
2. [Agression Datasets](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Aggression/4267550) Version 5

## Directory Structure
```bash
├── Visualizations (all visualizations plotted for this analysis)
├── tsv (all data files here for toxicity and aggression corpus from wikipedia talks)
├── 'a2- bias in data.ipynbs'
├── README.md
├── LICENSE

```

## Features
1. This analysis analyze the comments collected from Wikipedia Talk corpus and labelled by at least 10 crowd-sourced workers.
2. There are 3 tsv for each hostile speech (Toxicity and Aggression).
3. We evaluated different types of bias in labelling the comments:<br/>
      a. Self Selection Bias (worker's parcipitation bias)  <br/>
      b. Response Bias ( worker's different interpretation of toxicity and aggression)  <br/>
4. Identifying conflicts in different hostile speech i.e. toxicity vs aggression.

## Conclusion
Research question 1.: We did find self selection bias in dataset but the bias is not leaked to response bias as per the analysis. We did not find demographic bias in labelling the comments for toxicity hostile speech.

Research question 2.: We did find examples of comments that are labelled as aggressive but not toxic and vice-versa. We compiled the list of words that makes the comments hostile speech but could not reach to conclusion, as the frequent words coming out to common in both hostile speech's comment. The hypothesis is that it could be the way comments are sentenced, leads to toxic or aggressive. 

## Final Visualizations
Distribution of workers who participated in labeling the comments by different demographic dimensions:

![Distribution of workers by different demographic dimensions](https://github.com/Arora-Dhruv/data-512/blob/main/data-512-a2/Visualizations/Workers%20participations.png)

Worker's average score of toxicity by different demographic dimensions:

![Distribution of workers by different demographic dimensions](https://github.com/Arora-Dhruv/data-512/blob/main/data-512-a2/Visualizations/Workers%20average%20score%20of%20all%20comments.png)

Word Cloud for comments which are labelled TOXIC by majority but not considered AGGRESIVE by majority:

![Word Cloud](https://github.com/Arora-Dhruv/data-512/blob/main/data-512-a2/Visualizations/Word%20Cloud%20from%20TOXIC%20comments%20that%20are%20not%20AGGRESSIVE.png)

### Main Requirements
* [Python](https://www.python.org/)- version 3.6
* Before installing we recommend setting up a clean [virtual enironment](https://docs.python.org/3.6/tutorial/venv.html).
  
### License
This project is available under the [MIT License](https://github.com/Arora-Dhruv/data-512/blob/main/data-512-a2/LICENSE)

[Wikimedia](https://foundation.wikimedia.org/wiki/Terms_of_Use/en) Terms of use
