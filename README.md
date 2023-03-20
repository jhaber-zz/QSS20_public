# QSS20 slides and activities

This public repo has content for the Fall 2022 iteration of `QSS20: Modern Statistical Computing` at Dartmouth College. The main components are slides and associated Jupyter notebook-based activities to practice Python or other concepts. The sections and skills covered are as follows.


## Python basics

  - **Activity**: [00_introclass.ipynb](activities/00_introclass.ipynb)
  - **Slides**: [02_qss20_w23_pythonbasics.pdf](slides/02_qss20_w23_pythonbasics.pdf)
  - **Concepts covered**: 
    - Variables and types
    - Lists
    - List comprehension
    - Numpy arrays


## Data wrangling and visualization

### Introduction to pandas for data wrangling
  - **Activity**: [01_pandas_blank.ipynb](activities/01_pandas_blank.ipynb)
  - **Solutions**: [01_pandas_solutions.ipynb](activities/solutions/01_pandas_solutions.ipynb)
  - **Data**: DC crime reports in 2020
  - **Slides**: [03_qss20_w23_pandas.pdf](slides/03_qss20_w23_pandas.pdf)
  - **Concepts covered**:
    - Aggregation using `groupby` and `agg`
    - Lambda functions within aggregation
    - Recoding variables using `np.where`
    - Recoding variables using `np.select`
    - Recoding variables using `map` and dictionary

### Visualization with `plotnine`
  - **Example code**: [01_plottingexamples_plotnine.ipynb](activities/01_plottingexamples_plotnine.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - Plotting using the `plotnine` wrapper for R's `ggplot2`
    - Types of plots covered: line graph; bar chart; facetted line; line grouped/colored by attribute

### User-defined functions
  - **Activity**: [02_functions_blank.ipynb](activities/02_functions_blank.ipynb)
  - **Solutions**: [02_functions_solutions.ipynb](activities/solutions/02_functions_solutions.ipynb)
  - **Data**: DC crime reports in 2020
  - **Slides**: [04_qss20_w23_userdefinedfunctions_latex.pdf](slides/04_qss20_w23_userdefinedfunctions_latex.pdf)
  - **Concepts covered**:
    - user-defined function to find matches within a broader pool of data
    - using list comprehension to apply a function iteratively over list elements


## Workflow tools

### LaTeX
  - **Activity**: [02_latex_output_examples_blank.ipynb](activities/02_latex_output_examples_blank.ipynb)
  - **Solutions**: [02_latex_output_examples_solutions.ipynb](activities/solutions/02_latex_output_examples_solutions.ipynb)
  - **Slides**: [04_qss20_w23_uderdefinedfunctions_latex.pdf](slides/04_qss20_w23_userdefinedfunctions_latex.pdf)
  - **Concepts covered**:
    - LaTeX and Overleaf syntax and workflow
    - Exporting tables from pandas to LaTeX

### Shell and git
  - **Slides with activities**: [05_qss20_w23_workflow.pdf](slides/05_qss20_w23_workflow.pdf)
  - **Concepts covered**:
    - Cloning and committing from git on command line (shell)
    - Manipulating files from command line


## Merging and regular expressions

### Exact merging and reshaping
  - **Activity**: [03_reshaping_merging_blank.ipynb](activities/03_reshaping_merging_blank.ipynb)
  - **Solutions**: [03_reshaping_merging_solutions.ipynb](activities/solutions/03_reshaping_merging_solutions.ipynb)
  - **Helper code** (used for data prep): [03_helper_merging_dataprep.ipynb](activities/solutions/03_helper_merging_dataprep.ipynb)
  - **Data**: San Diego business tax certificate data; Census NAICS code data
  - **Slides**: [06_qss20_w23_mergereshape.pdf](slides/06_qss20_w23_mergereshape.pdf)
  - **Concepts covered**:
    - Converting wide to long data formats (melt) and long to wide (pivot)
    - Data cleaning such as extraneous rows/columns
    - Recasting join cols to allow join (e.g., converting `int` to character)
    - `pd.merge` and different types of exact joins using join keys
    - Post-merge diagnostics

### Regular expressions
  - **Activity**: [04_regex_blank.ipynb](activities/04_regex_blank.ipynb)
  - **Solutions**: [04_regex_solutions.ipynb](activities/solutions/04_regex_solutions.ipynb)
  - **Helper code** (used for data prep): [04_helper_regex.ipynb](activities/solutions/04_helper_regex.ipynb)
  - **Data**: Food Research Action Center (FRAC) [data on district and school's election of community eligibility provision (CEP)](https://frac.org/research/resource-library/community-eligibility-cep-database) for Free or Reduced Price Lunch (FRPL)
  - **Slides**: [08_qss20_w23_regex.pdf](slides/08_qss20_w23_regex.pdf)
  - **Concepts covered**: 
     - Pattern construction using `re` module
     - `re.sub` for replacement
     - `re.findall` 
     - `re.match` and how to work with match objects using `.group()`
     - Throughout, review of list comprehension 
  


## Text as data

### Introduction to text mining
  - **Activity**: [05_textasdata_partI_textmining.ipynb](activities/05_textasdata_partI_textmining.ipynb)
  - **Solutions**: [05_textasdata_partI_textmining_solutions.ipynb](activities/solutions/05_textasdata_partI_textmining_solutions.ipynb)
  - **Data**: simplified data from airbnb NYC listings. Stored in `public_data/airbnb_text.zip`
  - **Slides**: part 1 of [09_qss20_w23_textasdata.pdf](slides/09_qss20_w23_textasdata.pdf)
  - **Concepts covered**:
    - Scoring based on dictionary of words
    - Part of speech tagging using `nltk`
    - Named entity tagging using `spaCy`
    - Sentiment analysis using `VADER`
   

### Topic modeling
  - **Activity**: [05_textasdata_partII_topicmodeling.ipynb](activities/05_textasdata_partII_topicmodeling.ipynb)
  - **Solutions**: [05_textasdata_partII_topicmodeling_solutions.ipynb](activities/solutions/05_textasdata_partII_topicmodeling_solutions.ipynb)
  - **Data**: simplified airbnb listings
  - **Slides**: part 2 of [09_qss20_w23_textasdata.pdf](slides/09_qss20_w23_textasdata.pdf)
  - **Concepts covered**:
    - Using `sklearn` to create a unigram document-term matrix
    - LDA topic modeling using `gensim`
    - Visualizing topics 
    - Obtaining top words per topic using `gensim`
    - Obtaining document-level topic probabilities using `gensim`


## APIs and web-scraping

### Introduction to APIs: [NAEP Data Service API](https://www.nationsreportcard.gov/api_documentation.aspx); [Yelp API](https://docs.developer.yelp.com/docs/overview)
  - **Activity**: [06_apis_blank.ipynb](activities/06_apis_blank.ipynb)
  - **Solutions**: [06_apis_solutions.ipynb](activities/solutions/06_apis_solutions.ipynb)
  - **APIs**: NAEP data explorer; Yelp API
  - **Slides**: [10_qss20_w23_APIs.pdf](slides/10_qss20_w23_APIs.pdf)
  - **Concepts covered**:
    - Writing a query
    - Using `requests` to execute a query and return a response
    - Processing a response
    - NAEP API for student test scores over time and geography
    - Yelp Fusion API business search and reviews endpoints

### Twitter API with `tweepy` wrapper
We didn't cover this in class this quarter because [the Twitter API is no longer free to use](https://twitter.com/TwitterDev/status/1621026986784337922?s=20). See [the Twitter API docs](https://developer.twitter.com/en/docs/twitter-api/getting-started/about-twitter-api) for updated info. This template code is provided as a starting point for students pursuing further research with the Twitter API.
  - **Example code**: [06_apis_partII_twitter_examplecode.ipynb](activities/solutions/06_apis_partII_twitter_examplecode.ipynb)

### Introduction to web-scraping
  - **Activity**: [07_scraping_blank.ipynb](activities/07_scraping_blank.ipynb)
  - **Solutions**: [07_scraping_solutions.ipynb](activities/solutions/07_scraping_solutions.ipynb)
  - **Data**: 
  - **Slides**: [11_qss20_w23_webscraping.pdf](slides/11_qss20_w23_webscraping.pdf)
  - **Concepts covered**:
    - Researching the digital era
    - Web-scraping decision hierarchy
    - Parsing HTML with `BeautifulSoup`
    - Scraping URLs with automated Google search
    - Using exclusion lists to filter HTML and URLs


## Supervised machine learning (ML)

### Introduction to supervised ML
  - **Activity**: [08_ML_intro_activity_blank.ipynb](activities/08_ML_intro_activity_blank.ipynb)
  - **Solutions**: [08_ML_intro_activity_solutions.ipynb](activities/solutions/08_ML_intro_activity_solutions.ipynb)
  - **Data**: Unstructured yelp reviews with labeled sentiment scores
  - **Slides**: part 1 of [12_qss20_w23_supervisedML.pdf](slides/12_qss20_w23_supervisedML.pdf)
  - **Concepts covered**:
    - Identifying text features for binary classification
    - Preprocessing to prepare for model training
    - Logistic regression
    - Train-test split
    - Metrics for ML model evaluation

### Decision trees and optimization
  - **Activity**: [08_ML_optimization_activity_blank.ipynb](activities/08_ML_optimization_activity_blank.ipynb)
  - **Solutions**: [08_ML_optimization_activity_solutions.ipynb](activities/08_ML_optimization_activity_solutions.ipynb)
  - **Data**: Tweets containing customer reviews of airlines
  - **Slides**: part 2 of [12_qss20_w23_supervisedML.pdf](slides/12_qss20_w23_supervisedML.pdf)
  - **Concepts covered**:
    - Methods for avoiding overfitting
    - Optimization/hyperparameter tuning
    - Tree-based methods
    - Cross-validation


## Introduction to SQL

  - **Example code**: [09_SQL_examplecode.ipynb](activities/solutions/09_SQL_examplecode.ipynb)
  - **Activity**: [09_SQL_activity_blank.ipynb](activities/09_SQL_activity_blank.ipynb)
  - **Solutions**: [09_SQL_activity_solutions.ipynb](activities/09_SQL_activity_solutions.ipynb)
  - **Data**: database form of Cook County SAO sentencing data. Two tables: `caseinit` (case initiations); `divert` (case diversions)
  - **Slides**: [13_qss20_w23_SQL.pdf](slides/13_qss20_w23_SQL.pdf)
  - **Concepts covered**:
    - Row and column filtering
    - Subqueries
    - Group by/aggregation
    - Basic joins/column and table aliasing
