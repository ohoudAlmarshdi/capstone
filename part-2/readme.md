# Part 2: Problem Statement, EDA and Dataset

## Overview

In this section you will update us on your project, including the project you have chosen, your problem statement, an extensive outline of EDA and modeling to date, the goal of your predictive model, and the data you will use to explore that model. 

**Your data must be fully in hand by this point OR you must have a solid, achievable plan to do so that has been communicated to your local instructor.**

We expect a formatted and complete Jupyter Notebook which accomplishes the following:

- Identifies which of the three proposals you outlined in your lightning talk you have chosen
- Articulates the main goal of your project (your problem statement)
- Outlines your proposed methods and models
- Defines the risks & assumptions of your data 
- Revises initial goals & success criteria, as needed
- Documents your data source
- Performs & summarizes preliminary EDA of your data

## Clearly refine your Problem Statement

Your problem statement should the guiding principle for your project.  You can think about this as a "SMART" goal.

- Specific: 
  - What precisely do you plan to do?
  - What type of model will you need to develop?
- Measurable: 
  - What metrics will you be using to assess performance? 
  - MSE? Accuracy? Precision? AUC?
- Achievable: 
  - Is your project appropriately scoped?
  - Is it too aggressive?  Too easy?
  - *Note:* If your project is too big, break it up into smaller pieces.  Sometimes a good project is the simply one part of a larger, longer-term agenda.
- Relevant:
  - Does anyone care about this?
  - Why should people be interested in your results?
  - What value will the completion of your project be adding?
- Time-bound
  - What's your deadline?

---

- **BAD**: I will model emergency room visits.
- **GOOD**: I will build a regression model to predict the number of daily emergency room visits for St. Someone's Hospital.  Model performance will be guided by RMSE, and the model should at least improve upon baseline by 10%.  Baseline is defined as the monthly average of visits over the last 10 years.

---

- **BAD**: I will investigate the aftermarket pricing of sneakers.
- **GOOD**: Specific image and text features of sports sneakers are predictive of determinding wether they will sell for more or less in the aftermarket.  The guiding metric will be area under the ROC curve.

---

- **BAD**: I will explore the link between obesity and blood pressure.
- **GOOD**: I will quantify the association between obesity and blood pressure through regression modeling.
- **BETTER**: As obesity increases, how does blood pressure change?
---

- **BAD**: I will predict that sources of news are liberal or conservative.
- **GOOD**:  I will look at text features to undersatnd how news can be classified as liberal or conservative.
- **BETTER**: Specific text feature frequencies can determine the broader category of news sources using classification.  I will describe what makes each class charactitaristically unique, describe what is both certain and uncertain using precision and recall as success metrics.  Then I will conclude with a description of "why" my model describes potential to predict these two categories.

---

## Data Guidelines

What should you thinking about and looking for as you collect your capstone data?

- Source and format your data
  - Have a way to save data locally (e.g., SQL or CSV), especially if scraping from the web or collecting from an API.
  - Create a data dictionary to accompany your data.
- Perform initial cleaning and munging.
  - Organize your data relevant to your project goals.
  - Write functions to automatically clean and munge data as necessary.
  - Take copious notes, for both others and yourself, describing your assumptions and approach.


## EDA Guidelines

Think about the following as you perform your initial EDA.

- Identify the data types you are working with.
- Examine the distributions of your data, numerically and/or visually.
- Identify outliers.
- Identify missing data and look for patterns of missing data.
- Describe how your EDA will inform your modeling decisions and process.
  

## Necessary Deliverables / Submission

Your code and technical notebook should be posted to your forked repo by OCtober 14th. I also recommend that at the end of this course, you create youre own personal github and push your proejct to that for potential employers to reference. 

 Materials must be presented in a Jupyter Notebook stored within a repository on your personal (*not* GA) GitHub. Please submit a link to this repository by the due date ([submission link](https://docs.google.com/forms/d/e/1FAIpQLScez-8PsyIgP548fNtsoDpuNTdKxsr6tVvKPDtbr-mQov6NCw/viewform?usp=sf_link)).
 
 
## Requirements

1. An executive summary:
  - What is your goal?
  - Where did you get your data?
  - What are your metrics?
  - What were your findings?
  - What risks/limitations/assumptions affect these findings?
2. Summarize your statistical analysis, including:
  - implementation
  - evaluation
  - inference
3. Clearly document and label each section of your notebook(s)
  - Logically organize your information in a persuasive, informative manner.
  - Include notebook headers and subheaders, as well as clearly formatted markdown for all written components.
  - Include graphs/plots/visualizations with clear labels.
  - Comment and explain the purpose of each major section/subsection of your code.
  - Document your code for your future self, as if another person needed to replicate your approach.
4. Clearly document all of your decision points in the relevant sections
  - How did you acquire your data?
  - How did you transform or engineer your data?  Why?
  ##### these next you will fill out by end of capstone
  - How did you select your model?
  - How did you optimize hyperparameters?
5. Host your notebook and any other materials in your forked Github Repository.
  - You repo should have README file that guides us through the repository and links to important files.
  - Include links and explanations to any outside libraries or source code used.
  - Host a copy of your dataset or include a link to a remotely hosted version.
  
### Best Practices

1. The README
  - The README is the landing page of your repo.  
  - It should start with a summary of what the repo contains and provide links to important files.
  - Think of it as a table of contents for your repo.
  - You should list the external libraries/packages that you use, especially if they are not standard (i.e., not part of the base Anaconda distribution.)
  - If you wrote a blog about this project, link to it from your README.
  - Include your website, twitter handle, etc., if you would like.
2. Organizing your repo
  - If you have multiple notebooks, start each filename with a number to assist in organization.
  - Give you notebooks descriptive filenames.  For example,
    - `1_Scraping.ipynb`
    - `2_EDA.ipynb`
    - `3_Model_Development.ipynb`
  - Keep data files in a single folder off the "root" of the repo.
  - Keep documentation/reports in a dedicated folder (like data).
  - If you have any other resources (images or PDFs), keep them in a dedicated folder (called `assets`, for example.)
3. Jupyter Notebooks
  - Data science is a non-linear, iterative process, but your final notebook should contain a linear "narrative."
  - Notebooks should be reproducible, which means that I will get the _same results_ as you did if I clone your repo and run your notebook.  Consider the following:
    - Is your data stored in the repo or available via a link?
    - If you use _any_ (_ANY_) random numbers anywhere, do you have a random seed so that you **always** get the same result?
    - Is your notebook 100% free of runtime errors?
    - In short, if I open your notebook and click "Cell -> Run All", will your notebook run completely, without errors and give me the same result _evert_ time?
    
 
## Useful Resources
 
- [Best practices for data documentation](https://www.dataone.org/all-best-practices) 
- [Describing data visually](http://www.statisticsviews.com/details/feature/6314441/Visualising-Statistics-The-importance-of-seeing-not-just-describing-data.html)
- [WSJ Guide to Information Graphics (book)](https://www.amazon.com/Street-Journal-Guide-Information-Graphics/dp/0393347281)
- [Storytelling with Data (book)](https://www.amazon.com/Storytelling-Data-Visualization-Business-Professionals/dp/1119002257/)
