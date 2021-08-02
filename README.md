# donor_choose_dataset
DonorsChoose.org receives hundreds of thousands of project proposals each year for classroom projects in need of funding. Right now, a large number of volunteers is needed to manually screen each submission before it's approved to be posted on the DonorsChoose.org website.

Next year, DonorsChoose.org expects to receive close to 500,000 project proposals. As a result, there are three main problems they need to solve:

1. How to scale current manual processes and resources to screen 500,000 projects so that they can be posted as quickly and as efficiently as possible
2. How to increase the consistency of project vetting across different volunteers to improve the experience for teachers
3. How to focus volunteer time on the applications that need the most assistance

The goal of the competition is to predict whether or not a DonorsChoose.org project proposal submitted by a teacher will be approved, using the text of project descriptions as well as additional metadata about the project, teacher, and school. DonorsChoose.org can then use this information to identify projects most likely to need further review before approval.

### Naive Bayes
For the given problem following operations are performed :
* Featurization :
    - Set 1: categorical, numerical features + preprocessed_eassay (BOW)
    - Set 2: categorical, numerical features + preprocessed_eassay (TFIDF)
* Hyperparameter tuning
* Training model with best hyperparameter 
* Summarizing the results

## Decision Tree
Part1 
For this model the following operations are performed on the provided dataset:
* Featurization:
    - Set 1: categorical, numerical features + preprocessed_eassay (BOW)
    - Set 2: categorical, numerical features + preprocessed_eassay (TFIDF)
* Hyperparameter tuning
* Training model with best hyperparameter 
* Summarizing the results
Part 2 
* selecting features which are having non-zero feature importance
* Trainging machine learning model on these features
* Comparing and summarizing the results

## GBDT
For this model the following operations are performed:
* Featurization:
    - Set 1: categorical(response coding use probability values), 
            numerical features + project_title(TFIDF)+
            preprocessed_eassay (TFIDF)+sentiment Score of eassay
    - Set 2: categorical( response coding use probability values), 
            numerical features + project_title(TFIDF W2V)+ 
                preprocessed_eassay (TFIDF W2V)
* Hyperparameter tuning
* Training model with best hyperparameter 
* Summarizing the results


