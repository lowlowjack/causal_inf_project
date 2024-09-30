# Case Study: Causal inferencing on E-commerce data

![Causal flow](/assets/dag_shared.jpg "Causal flow")

## Goal

Based on the data, devise a data-backed strategy that will help guide the business and lead to higher revenue based on sensible metric optimization. 

## Background

This dataset has been obtained from Kaggle and contains e-commerce transactions data of an electronics vendor from 2015-2016 in India. Also included is high level marketing spend of the firm during this period as well. This choice of data was to illustrate how one can still infer conclusions even if the information is limited, or when machine learning and predictive abilities are limited. 

The raw dataset used for this analysis can be obtained from [Kaggle](https://www.kaggle.com/datasets/datatattle/dt-mart-market-mix-modeling) 

## Work

I've structured the work into a few sections.

1. A brief write up on the methodology to understand how one looks at the background problem. **It is recommended to start reading this before diving into the technical details.** 
2. A presentation summary that discusses the findings and how we translate those to the business context. *For those, who do not wish to know technical details and just want to understand applications, start here.*
3. Notebooks that describe the details.

- For more on the methodology: [blog page](https://lowlowjack.github.io/2024-09-29-going-from-analytics-to-science/).
- For a presentation summary of results: [Google Slides](https://docs.google.com/presentation/d/1nncf-fzmn0jox9lDAzNZjUyxRQ0v1vJn9shwO0JnfbA/edit?usp=sharing)

The rough idea on methodology is that it uses a mixture of different models to attempt to try to create an observational study group that we can draw inferences on. 

There are three notebooks in the repo that derive the working to the presentation and put the methodology in action. To re-run the notebooks, the requirements.txt should have the correct setup of repos to prevent library issues. **PLEASE ensure that you're on Python 3.11. The repos will not work on Python 3.12**. The notebooks shuold be read in the following order.

1. **data_cleaning.ipynb**: Notebook that cleans the data into our models and notes a few observations before modelling. 
2. **bayes_mm_validation.ipynb**: Notebook that creates a mixed model that aims to motivate and validate some of the results we will observe in SCM modelling in the first notebook. Some knowledge of Bayesian statistics would be useful to have before reading here, but I've linked a few resources that can help get people up to speed inside the notebook.
3. **causal_inf_main.ipynb**: Main notebook that uses structural causal models (SCMs) to model causal relations between different features that we are observing. 

## Tips and Guidance
- If some of the technical details of the work may be difficult to understand, (e.g. Why one mechanism is used, how said mechanism works), try to grasp the high level flow first and then come back to understand how the details accomplish the goal. I would be happy to clarify the details over a chat or email.
- I've omitted some of the larger data files in the writeup. For raw data, they may be downloaded from Kaggle. For the processed data, you may contact me for those. 
- For any other inquiries, please chat over: https://www.linkedin.com/in/jack-low-667468b6/ 