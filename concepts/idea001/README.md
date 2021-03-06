### Data Collection
First we need the job ads for classification which we can get from Talent API(paid). There is a free dataset available on Kaggle 
[Online Job Postings](https://www.kaggle.com/madhab/jobposts) which can be used.
[Indeed Internships](https://download.data.world/file_download/rdowns26/marketing-internship-postings/internships_on_indeed.csv)
[Internships](https://download.data.world/file_download/rdowns26/marketing-internship-postings/internships_not_on_indeed.csv)
[NYC JOBS](https://data.cityofnewyork.us/City-Government/NYC-Jobs/kpav-sd4t)

### Classification Algorithms
Two main categories of classification algorithms used in AI are SVM under machine learning and LSTM or BLSTM under AI.
We can use two main classification techniques which can be used for classify ads.
```text
1 - Using classic algorithms like Random Forests or SVM
2 - Using Recurrent Neural Networks such as LSTM, BLSTM
```

### Small dataset
If dataset consists of 1000-5000 ads then we have to use SVM, Random Forests.
Data is already in proper format, some important features of ads would be
```text
- location
- requirements
- title
- tasks
- company
```

Model will out one of the following class for classification of ads
```text
FULL_TIME
PART_TIME
CONTRACTOR
TEMPORARY
INTERN
VOLUNTEER
PER_DIEM
OTHER
```
We can use SVM or Random Forests for classification on small dataset.
### Large Dataset
If dataset has more than 10000 records of ads then LSTM or BLSTM is the best choice for classification. For RNN, text classification 
approach is best for classifying ads. `requirements` is the most important feature for job ads which provides necessary information
about the kind of the job. 