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

The goal is to create a Jupyter notebook that  contains your data preparation, analysis, and visualizations for all the time series data that the company needs to understand. Text and comments to document my findings, and answered the question prompts in the instructions, plot the results so that we can visually show illustrate the predictions.


[
<img width="647" alt="Screen Shot 2021-06-07 at 6 17 15 PM" src="https://user-images.githubusercontent.com/80833988/121107334-986d2180-c7bc-11eb-9d10-f2e0ece08fea.png">
](url)


## Software version control


### Libraries 
*  Pandas - is a software library designed for data analytics that makes it easier to work with data from practically any type of file. Pandas supplies powerful tools for working with time data in particular, and time is a key aspect of financial analysis. Analysts typically compare and measure financial assets—from single stocks to large portfolios—across time.
*  Prophet - is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.
* Following libraries were imported

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
Particularly in "Step 1: Find Unusual Patterns in Hourly Google Search Traffic"

```
# Upload the "google_hourly_search_trends.csv" file into Colab, then store in a Pandas DataFrame
# Set the "Date" column as the Datetime Index.


df_mercado_trends = Path("google_hourly_search_trends.csv")
df_mercado_trends = pd.read_csv(df_mercado_trends, index_col='Date', infer_datetime_format=True, parse_dates=True)
```


[
<img width="998" alt="Screen Shot 2021-06-07 at 9 56 59 PM" src="https://user-images.githubusercontent.com/80833988/121125361-4b4c7800-c7db-11eb-8a00-778394f414ab.png">
](url)

and "Step 3: Relate the Search Traffic to Stock Price Patterns"

```
# Upload the "mercado_stock_price.csv" file into Colab, then store in a Pandas DataFrame
# Set the "date" column as the Datetime Index.

df_mercado_stock = Path("mercado_stock_price.csv")
df_mercado_stock = pd.read_csv(df_mercado_stock, index_col='date', infer_datetime_format=True, parse_dates=True)
```

[
<img width="1024" alt="Screen Shot 2021-06-07 at 10 00 02 PM" src="https://user-images.githubusercontent.com/80833988/121125637-b9913a80-c7db-11eb-930f-af3e5b03c9cf.png">
](url)



### Results and summary of the analysis

Step 1.
[
<img width="1029" alt="Screen Shot 2021-06-07 at 10 04 19 PM" src="https://user-images.githubusercontent.com/80833988/121126006-50f68d80-c7dc-11eb-8330-ce86fe0b07a6.png">
](url)


Step 2.

[
<img width="1057" alt="Screen Shot 2021-06-07 at 10 05 12 PM" src="https://user-images.githubusercontent.com/80833988/121126080-71264c80-c7dc-11eb-8a4f-bd21b416300a.png">
](url)

Step 3.

[
<img width="1127" alt="Screen Shot 2021-06-07 at 10 06 26 PM" src="https://user-images.githubusercontent.com/80833988/121126184-9ca93700-c7dc-11eb-9d03-b54b4197905d.png">
](url)

Step 4. 

[
<img width="960" alt="Screen Shot 2021-06-07 at 10 08 14 PM" src="https://user-images.githubusercontent.com/80833988/121126346-dd08b500-c7dc-11eb-8c48-73c1009fd72b.png">
](url)

Explore the correlation:

[
<img width="958" alt="Screen Shot 2021-06-07 at 10 08 58 PM" src="https://user-images.githubusercontent.com/80833988/121126421-f873c000-c7dc-11eb-976c-ccede0e76c57.png">
](url)

Forcast with Prophet

[
<img width="973" alt="Screen Shot 2021-06-07 at 10 09 53 PM" src="https://user-images.githubusercontent.com/80833988/121126503-18a37f00-c7dd-11eb-9c4e-2a7510a8c928.png">
](url)

Slice and explore the data:

[
<img width="808" alt="Screen Shot 2021-06-07 at 10 12 18 PM" src="https://user-images.githubusercontent.com/80833988/121126692-6e782700-c7dd-11eb-808a-62f597a021d6.png">
](url)

[
<img width="979" alt="Screen Shot 2021-06-07 at 10 10 46 PM" src="https://user-images.githubusercontent.com/80833988/121126567-37a21100-c7dd-11eb-9b96-522d2a89998b.png">
](url)

## Helps recruiters

The project was created in collaboration with Berkeley Fintech Bootcamp team: Allan Hall, Joel Gonzales.

Tutor Lavina Tang helped me to polish my code and tought me how to run separate parts of code to see if it works every step.

AskBCS Learning Assistant channel was used to troubleshoot some of the accuring problems outside of the classroom

## License

MIT
