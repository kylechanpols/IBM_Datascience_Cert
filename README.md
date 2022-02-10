# IBM Data Science Capstone: Determining mission outcomes in SpaceX's Falcon-9 Landings

Welcome to the repository of my jupyter notebook and code for the final project of the IBM Data Science Professional Certificate. Here you will find code used to generate results reported in the final project.

![](https://kylechanhy.netlify.app/media/Untitled2.jpg)
![](https://kylechanhy.netlify.app/media/Untitled4.jpg)

The final report is available as a PDF, namely `Final report.pdf` in the repository.

## Project Description

The project aims to find out the determinants of a successful first-stage landing of SpaceX's Falcon-9 project. 

According to SpaceX, Falcon 9 cost around $62 mil, which is less than half of other rocket providers

- The cost saving comes from the fact that the first-stage Falcon 9 rockets can be
reused
-**Business Problem Statement**
-- How costly is a Falcon-9 rocket launch? If we can predict whether the first stage will land, we
can determine the cost of a launch easily.
-- How can we improve the success rate of the first-stage? If we can improve further, we might be able save even more by increasing the re-use rate of the first-stage rockets.

## Project Outcome

- EDAs and subsequent analyses using interactive dashboards (Dash) show that **payload** mass and **Orbit type** are the most important factors in determining mission success.
- Based on these results, 4 different models were developed and tested. Eventually I chose a simple Logistic Regression model with L2 regularization as the model of choice. The model has the highest accuracy score on the test set and is the most simple among other alterntives. 

## Code

`01-jupyter-labs-spacex-data-collection-api.ipynb` - Data Collection Jupyter Notebook - This notebook walks through how I collected data from the SpaceX API.

`03-labs-jupyter-spacex-Data wrangling.ipynb` - The Data Wrangling Notebook - This notebook walks through the steps I've taken to clean the data, encode features using one-hot encoding, and standardize the data.

`04-jupyter-labs-eda-sql-coursera.ipynb` - SQL Notebook - This notebook walks through the steps I've taken to get summaries of the data using SQL. The data is stored on an IBM DB2 instance and I used Python (with the `sql` extension) as an interace to evaluate SQL queries.

`05-jupyter-labs-eda-dataviz.ipynb` - EDA Notebook - This notebook walks through the steps I've taken to generate data visualization (matplotlib, seaborn) to help guide the EDA process.

`06-Final Capstone - Dashboard.ipynb` - Mapping Notebook - This notebook plots the geographical features in the dataset and visualize the relationship between these features and mission outcomes on an interactive map (Folium).

As Github does not render Folium maps, a fully interactive rendered notebook is available [here](https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/1b101bbb-59ab-4e75-bc79-a969facda46d/view?access_token=69b0ea8214f5334ee0c67469782c4decdfbbe57d5aa791eeecc9616a78cdeb35).

![](https://kylechanhy.netlify.app/media/Untitled3.jpg)
![](https://kylechanhy.netlify.app/media/Untitled4.jpg)

`07-Final- Dash.py` - Dashboard Script - This script launches an interactive dashboard (built with `Dash`) to allow users visualize:

1. Share of success rates across launch sites
2. Success-to-failure ratios in different launch sites
3. Relationship between payload mass and success likelihood across different launch sites.

![](https://kylechanhy.netlify.app/media/Untitled1.jpg)
![](https://kylechanhy.netlify.app/media/Untitled2.jpg)

`08-SpaceX_Machine Learning Prediction_Part_5.ipynb` - Model Development Notebook - This notebook shows how I developed the four models, tuned them with the best model parameters, and compared their performance.

