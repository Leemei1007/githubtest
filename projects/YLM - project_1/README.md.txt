## Scenario

A client which is a Singapore-based company, is in the business of private tutoring (both online and in-class tutor). The client has been providing SATS private tutoring to international school students in Singapore who adopt the USA education syllabus and the client's method of teaching and contents have been well received and regarded. In view of such resounding success, the client now wishes to expand its online tutoring for SATS in the USA. As the client is relatively unknown outside of Singapore, for a start, it has to invest in advertising its business. As advertising throughout the whole USA can be costly, the client is asking for advice which USA state should it target its advertising as part of its pilot programme? In addition, as part of its community service publicity, it has allocated some budget/financial aid to award scholarships to deserving students. 

## Problem Statement

1. To analyse which state is the most promising for the client to promote its services

2. Targeted states: states with the highest and lowest participation rate  

## Summary

### Import and clean data of SAT and median income in the USA for each state for 2017, 2018 and 2019
Errors such as extra characters were rectified, non-USA states were removed, numbers in string converted to float and percentages were removed to convert all numerical data in numbers with decimal points. Indexes were reset. 

Additional note - Year 2020 data was not chosen for analysis as the year 2020 was an unprecedented year. As each USA state was governed differently, for eg. not all states imposed lock downs and each test center made individual decisions about whether to administer the SAT, the year 2020 data may be skewed

### Exploratory Data Analysis
Assess which state has the highest and lowest participation rate and test scores

### Data Visualization
Histograms, boxplots, heat maps and scatterplots were used to investigate the data and correlations further. Some data appear to portray normal distribution (which is the total scores data)



### Outside Research
Additional searches were made to aid analysis

### Data Dictionary



|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|string|SAT|The states in the USA|
|sat_participation|float|SAT|The percentage expressed as a float on the number of students enrolled in schools|
|sat_read_write_scores|float|SAT|The average reading and writing score in a maximum score of 800|
|sat_math_scores|float|SAT|The average math score in a maximum score of 800|
|sat_total_scores|float|SAT|The combined score of sat_reading_and_writing and sat_math|



## Conclusions and Recommendations

**Key takeaways**

1. The states with the highest participation rate tend to be states which impose SAT as mandatory
2. Score wise, we observe that the higher the participation rate, the lower the average total SAT scores. States with highest participation rate tend to be states which imposed SAT as mandatory, hence the average score reflects performance of students of various capabilities (i.e. strong and weaker students). As for states whereby SAT is not mandatory, there is a high likelihood that only strong students participated, which may explain the tendency for these states to have higher average scores
3. Generally there is no trend between income and scores, which means that SAT scores were not influenced by the income of each state. However, this data may not be accurate because less well-to-do students may drop out of SAT (more so, in states where SAT is not mandatory) and hence, this data may be biased. 
3. Overall, there is an improvement in participation rates of SAT from 2017 to 2019 (with a compound annual growth rate of approximately 11%) as certain states made the move to impose SAT as mandatory. 

**Recommendations**

Our client should channel its budget in these states:   

|Budget|States selected|Basis|Justification|
|---|---|---|---|
|Advertising|Colorado, Connecticut, Delaware, Florida, Idaho, Illinois, Maine, Michigan, New Hampshire, Rhode Island, West Virginia|Top participating states 2017-2019 / States where SAT is compulsory|Large and stable market to advertise the client's business. As SAT is made compulsory, there is a chance for relatively high take-up rate and stable enrolment rate in the near term. Data shows that SAT participation grew at a compound annual growth rate of about 11% from 2017-2019|
|Advertising and scholarship/financial aid|Arkansas, Iowa, Kansas, Kentucky, Louisiana, Minnesota, Mississipi, Missouri, North Dakota, Nebraska, South Dakota, Utah, Wisconsin, Wyoming|Least participating states (also happened to be top scoring states 2017-2019)|These states are states where SAT is not compulsory. Hence, there is a likelihood that only stronger students participated, as depicted by the relatively high average scores compared to states with higher participation rates. Students in these states who are weaker or not financially able may shy away from SAT. Hence, there is a potential untapped market to be explored in these states. Scholarships/financial aid can be channeled to these states to entice more students to participate (and also enhance client's corporate image and boost publicity)|

