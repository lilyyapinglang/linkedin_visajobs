# linkedin_visajobs
This repository uses a linkedin job posting dataset from Kaggle (https://www.kaggle.com/datasets/mertguvencli/linkedin-jobs) to mainly analyse these questions of interests:
- Among Data engineers, Data Scientists, Machine Learning, and Data Scientists, Which job is most in demand in the job market?
- Which country or location has the most such job openings? It should somehow suggest this country actively developing in tech
- Which country or location has the most job openings that provide visa sponsorship worldwide talents? It should indicate which country is more open to international tech talents.
- Among those jobs that provide visa sponsorship, what are some general required skills/experiences?

The detailed analysis, thought processes and reults can be found in this Medium post. [Visa-friendly countries/locations for international Data Science professionals]( https://medium.com/@lilyyapinglang/visa-friendly-countries-locations-for-international-data-science-professionals-97989aef5a8c)
## Installation

### Python (>=3.7)
### Install needed python libraries 

```
pip install matplotlib
pip install sqlite3
pip install nltk
pip install ssl
pip install langdetect
pip install vaderSentiment
```

## Motivation for the projects

I’ve always wanted to explore a lifestyle as a digital nomad where you live and work in different places of your interests for a period of time. But be able to legally work in a place, you first need to look out for opportunities that sponsor visas or work permits. There are a vast amount of jobs being posted but it is just time-consuming to search, click one by one, look for the visa sponsor terms in the job description and then pick the ones that match that requirement. So I want to use a job posting dataset and perform text analysis on the Job Description visa-related text to quickly filter out the jobs that provide visa sponsorship and relocation support for international applicants. Once get the filtered result, in addition to looking at the job list, we can also derive some valuable clues as to which country/city is more open to global talents, and what are the most needed skill sets for these job opportunities. 

## File Descrptions
- `DS_Job_Visa.ipynb` includes all code, commands in order to get the same results as the medium post. Install needed libraries first and then run the notebook. 
- `linkdin.db`, contains 26k+ jobs scraped from Linkedin

## How to interact
1. Clone the repository to your local machine
2. Get the job dataset. Download the `linkedin.db` dataset from kaggle https://www.kaggle.com/datasets/mertguvencli/linkedin-jobs
3. Place the downloaded `linkedin.db` in the same folder as the `DS_Job_Visa.ipynb` of this repository
4. Install above mentioned needed python libraries.
5. Open an IDE of your choice to run through the `ipynb` to get the results

## Summary of Analysis
For Data Scientists, Data Engineer, Machine Learning or Software Engineer professionals who are interested in relocation and visa sponsoring opportunities to explore another country, among cities of these 11 regions (Germany, Netherlands, United States, France, United Kingdom, Poland, Canada, India, Brazil, Italy, England), targeting below mentioned cities and skillsets when preparing yourself for relocation could be a good bet:

**Job opportunities:**
Data Engineer > Software Engineer > Machine Learning > Data Scientist

**Top 5 Cities that has most visa-sponsoring jobs:**
Berlin> Amsterdam>Paris >Bengaluru(India)> Munich>Oxford

**Top 5 Countries that has most visa-sponsoring jobs:**
Germany>Netherlands>United States>United Kingdom> France

**Top 5 Skills/Experience required:**
- Framework: Docker > Pandas> Numpy > Tensorflow > Scikit Learn

- Platform: Microsoft Azure> Google Cloud >IBM> Amazon AWS

- Database: MySQL>Snowflake > Cassandra>ElasticSearch>MongoDB

- Languages: Python>SQL>Java>Go>R
## Licensing, Authors, Acknowledgements
Code and documentation copyright 2011–2022 lilyyapinglang. MIT License. 
