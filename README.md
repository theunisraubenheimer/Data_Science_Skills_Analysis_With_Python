# Data Science Skills Scraper
---
### Problem Background:
A common problem faced by data scientists, data engineers and data analysts, especially novices, are not being certain of which skills to learn to ace that interview, or to perform at your current DS, DE or DA job. 

I found dozens of articles and videos online, but the problem was I found it difficult to trust the advice coming from this content, as it might be filled with their personal bias, or just their personal opinion which might not reflect the true state of the skills needed in industry at the moment.

I also figured that bootcamps, university courses and MOOCs (Massive Open Online Courses) are business and they want to sell you a course, so they might also just be using the data science hype and buzzwords to sell you these courses.

After experiencing the same feeling and wanting to upskill myself with skills that are actually needed, I wanted to find a way to identify the skills that I need to learn to stay relevant that will eliminate bias and that will accurately identify these skills.

---
### Approach:
Focusing on an industry 'pull' methodology vs a bootcamp/university/MOOC 'push' methodology, a BeautifulSoup web-scraper was built that scrapes the jobs site Indeed for full-time, entry-level 'data scientist' job postings in the US. These job postings are then stored in a CSV file, and analysed with Python and the nltk and pandas packages.

#### Considerations and Assumptions to be aware of:
1. An assumption is made that the job postings and the subsequent skills listed in them accurately reflects what skills are needed by the specified job listed. A common occurence is where people that don't possess the necessary technical knowledge to create the job postings, create them. This needs to be considered. 
2. Duplicate words in each job description was removed. A total of 495 jobs were scraped, so any one word can not be counted more than 495 times in total. The logic is explained below.
3. The code in part 1 and part 2 was repeated for 'Data Engineer' and 'Data Analyst' job roles, in addition to the 'Data Scientist' job role illustrated in part 1 and part 2. It is not shown in this analysis, as it follows the exact same procedure stipulated in parts 1 and 2. 
---

## Results:
The following is a report created, based on the analysis in the code in this notebook.

It was created in Power BI, and is a static version of an interactive dashboard.

### Data Scientist Analysis Results:
![Banner](https://github.com/theunisraubenheimer/Data_Science_Skills_Analysis_With_Python/blob/main/The_Data_Scientist.png)

A few key insights:
- Python is king! It was mentioned 23% more times than R (59% vs 36%)
- Machine learning stays one of the top competencies needed for data scientists
- Data Scientists are educated: about 50% of job postings require a postgraduate degree
---

### Data Engineer Analysis Results:
![Banner](https://github.com/theunisraubenheimer/Data_Science_Skills_Analysis_With_Python/blob/main/The_Data_Engineer.png)

### Data Analyst Analysis Results:
![Banner](https://github.com/theunisraubenheimer/Data_Science_Skills_Analysis_With_Python/blob/main/The_Data_Analyst.png)

---

## Conclusion:
A very fun exercise, this project showcased the collection of data, the cleaning of data, the interpeting and analysis of data, and finally, the visualization of the results of the interpretation and analysis.

It showcased how to use a webscraper to extract data from a website, and how to use a logical approach to formulating a business problem (_which skills should a data scientist learn_) and finally solving the problem using a data-driven approach.

To solve the business problem: in order to be deemed a competent data scientist, based on 495 real companies' data scientists requirements, the skills one should focus on is python, statistics, statistical modelling, R, SQL, data visualization and cloud technologies, to name a few. The competencies one should focus on is being able to work in a team, machine learning and be in possession of a degree (ideally a postgraduate degree).

A noteworthy insight achieved from the analysis of the 'data scientist', 'data engineer' and 'data analyst' job postings, which included +-1200 roles and almost 1.2 million words, was that the word 'team' was in the top 3 of competencies mentioned in all three roles.

_Working with data is a team sport, let us never forget that._
