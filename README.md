
# Garanti BBVA Data Camp 


Garanti BBVA contributes to the economy and society with a digitalization and people-oriented vision, works with the understanding of 'we are one team' to provide the most advanced banking solutions to more than 19 million customers, and builds its operations on 'open, transparent and responsible banking' with its approximately 20,000 employees.

The expectation is:
As part of this competition, we expect you to predict whether people changed jobs in 2019 using the tech-talent dataset we shared.

The success metric in the Kaggle competition will be Categorization Accuracy. Participants who ranked in the top 10 on the Private Leaderboard will attend the final presentation on February 25, 2023, where they will explain their work to the jury.


## Attribute Information
The training set, the protein thermostability (experimental melting temperature) data includes natural sequences, as well as engineered sequences with single or multiple mutations upon the natural sequences. The data are mainly from different sources of published studies such as Meltome atlas—thermal proteome stability across the tree of life.

Education

● user_id - unique candidate id

● school_name - educational institution name

● degree - degree

● fields of study - section

● start_year_month - educational institution start date

● end_year_month - educational institution end date

languages

● user_id - unique candidate id

● language - language

● proficiency - level

skills

● user_id - unique candidate id

● skill - skill


work_experiences

● user_id - unique candidate id

● company_id - unique company id working with

● location - company location

● start_year_month - start date



## Acquirements

First, some values are disabled to avoid overfitting as they are from 2019. Since it is envisaged that the data in separate files will be preprocessed separately, approaches such as outlier cleaning for the datasets one by one, adding new variables and feature engineering were applied as it was thought that using the existing information would be of great benefit to the machine learning side.

At the same time, using data visualization libraries and approaches, the general distribution of the data was examined and the situation was informed. After examining the data separately, the applied changes were also applied to the test and train datasets. It was gathered under the name of a single dataset ("original_data"), and the model moved to the training (train,test) side. 

On the model training side, the Holdout method was initially tried, but it was observed to be prone to low scores even though it was tried with different models.Therefore, it was predicted to use StratifiedKFold method and it was realized that higher scores could be achieved.



