[
<img width="607" alt="Screen Shot 2021-06-07 at 6 13 12 PM" src="https://user-images.githubusercontent.com/80833988/121107043-0fee8100-c7bc-11eb-9671-a85fefb08d9d.png">
](url)



> "In this Challenge, I will assume the role of growth analyst at MercadoLibre-most popular e-commerce site in Latin America. With a task of analyzing the company's financial and user data i need to find a clever ways to make the company grow. Using my new skills of forecasting future with Prophet, i will try to predict search traffic and translate it into the ability to successfully trade the stock
"

# Forecasting
Forecasting With Prophet 


:star: Challenge 11

!!! Go to "How to install" in order to properly run the code.


## Table of content
- [Overview of the project and project goals](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#overview-of-the-project-and-project-goals) 
- [Software version control](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#software-version-control)
    - [Libraries / interfaces](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#libraries--interfaces)
    - [Work with GitHub](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#work-with-github)
    - [How to install](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#how-to-install)
- [Results and summary of the analysis](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#results-and-summary-of-the-analysis)
- [Helps recruiters](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#helps-recruiters)
- [License](https://github.com/nataliaburrey/crypto_investments/blob/main/README.md#license)





## Overview of the project and project goals

The goal is to create a Jupyter notebook that  contains your data preparation, analysis, and visualizations for all the time series data that the company needs to understand. You’ll use text and comments to document your findings, and you’ll answer the question prompts in the instructions. 
then plot the results so that we can visually show illustrate the predictions.


[
<img width="647" alt="Screen Shot 2021-06-07 at 6 17 15 PM" src="https://user-images.githubusercontent.com/80833988/121107334-986d2180-c7bc-11eb-9d10-f2e0ece08fea.png">
](url)


## Software version control


### Libraries 
*  Pandas - is a software library designed for data analytics that makes it easier to work with data from practically any type of file. Pandas supplies powerful tools for working with time data in particular, and time is a key aspect of financial analysis. Analysts typically compare and measure financial assets—from single stocks to large portfolios—across time.
*  Prophet - is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.
* Following libraries were used to analyze the data

```
# Import the required libraries and dependencies
import pandas as pd
from pathlib import Path
import holoviews as hv
from fbprophet import Prophet
import hvplot.pandas
import datetime as dt
%matplotlib inline
```

The following code is also promped us to install nesessary libriries right in google colab:

[
<img width="766" alt="Screen Shot 2021-06-07 at 6 20 56 PM" src="https://user-images.githubusercontent.com/80833988/121107631-1cbfa480-c7bd-11eb-8825-ab1c071e3975.png">
](url)

### Interfaces

- Google Colab
The Facebook Prophet library can be difficult to install on some machines, so in this module you'll also get aquainted with Google Colab - an IDE that allows you to run Jupyter Notebooks in the cloud.

 
### Work with GitHub
* Repository created on GitHub
* Files were  committed using command line
* Our repository is organized, and includes Resources folder with CSV  project files, 
* Jupyter Notebook with code runs without errors.
* Answers on nesassary questions are included

### How to install

* Save remote repo from GitHub to your computer (Desktop): in Terninal type:

```
cd desktop

git clone https://github.com/nataliaburrey/Forecasting.git
```

now you can find repo on your desktop


* We will run a Jupyter Notebook in [Google Colab](https://colab.research.google.com/) 
*  Choose [ forecasting_net_prophet.ipynb ] file in Forecasting folder to see the analysis report.


[
<img width="1313" alt="Screen Shot 2021-06-07 at 6 28 55 PM" src="https://user-images.githubusercontent.com/80833988/121108225-3ad9d480-c7be-11eb-8e60-fcb9152c4c53.png">
](url)

The following code in the document promts you to Choose appropriate CSV file to access the data 

```
from google.colab import files
uploaded = files.upload()

```






### Results and summary of the analysis



## Helps recruiters

The project was created in collaboration with Berkeley Fintech Bootcamp team: Allan Hall, Joel Gonzales
Tutor Lavina Tang helped me to polish my code and tought me how to run separate parts of code to see if it works every step.
AskBCS Learning Assistant channel was used to troubleshoot some of the accuring problems outside of the classroom

## License

MIT
