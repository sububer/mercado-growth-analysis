# mercado-growth-analysis
FinTech Challenge 11 -- MercadoLibre Growth and TimeSeries Analysis  

See full implementation and notebook details in [forecasting_net_prophet.ipynb](app/forecasting_net_prophet.ipynb)  

---

## Overview Of Analysis

MercadoLibre is a popular e-commerce site in Latin America. This is a multi-faceted analysis of the company's financial and user data, aimed at shedding insights which will help the company grow. 

At a high-level, the following will be performed:  
- visual depictions of seasonality based on Google Search trends
- evaluation of how stock price correlates to Google Search trends
- [Prophet](https://facebook.github.io/prophet/docs/quick_start.html#python-api) forecast model predicting hourly search traffic
- a plot of forecast for future company revenue  

See full implementation and notebook details in [forecasting_net_prophet.ipynb](app/forecasting_net_prophet.ipynb)  

---  

## DataSet Details  

Data sets used to anlyze this space:
- [google_hourly_search_trends.csv](data/google_hourly_search_trends.csv) hourly google trend data
    - contains data: `Date | Search Trends `  
- [mercado_daily_revenue.csv](data/mercado_daily_revenue.csv)
    - contains data: `date | Daily Sales `  
- [mercado_stock_price.csv](data/mercado_stock_price.csv)
    - contains data: `date | close `  

---  

## Results  

### Search Traffic Patterns

Mercado Libre released its quarterly results in May 2020. This month was isolated and analysed.  
The traffic in May 2020 was `38181`, which is `8.55%` higher than the median monthly traffic of `35172.5`.  

**Mercado Search Trends - May 2020**  
![May 2020 Search Results](media/01-search-traffic_patterns.png)

### Seasonality Mining From Search Data

Daily, hourly, and weekly seasonality was observed in the search data.  
`Daily` - Tues had the highest average search traffic, with Monday a close second.  
`Hourly` - The heatmap reveals that nearly every day, search traffic is highest from hour 22 to hour 01. Sunday however has a longer lull of low traffic from eary to mid day, but is still high by hour 23 at the day's end.  
`Weekly` - The search traffic does show a rise during weeks 40 to 52, rising from 45.3 in week 42 to 49.7 in week 51. Traffic drops at the very last/first week of the year.  

![Avg Traffic By Day Of Week](media/02-avg-traffic-by-day-of-week.png)  
![HeatMap Search DayOfWeek / Hour](media/03-heatmap-day-of-week-by-hr.png)  
![Avg Search Traffic by Week Of Year](media/04-avg-search-by-week-of-year.png)  


### Search Traffic to Stock Price Correlation

### Prophet Time Series Model

### Forecast Revenue From Time Series Model



See full implementation and notebook details in [forecasting_net_prophet.ipynb](app/forecasting_net_prophet.ipynb)  

## Summary   

TBD


---

## Technologies

This challenge uses [python](https://www.python.org/) 3.7 and the following [built-in](https://docs.python.org/3/py-modindex.html) modules:
- [os](https://docs.python.org/3/library/os.html#module-os)
- [pathlib](https://docs.python.org/3/library/pathlib.html)
- [datetime](https://docs.python.org/3/library/datetime.html)

Additionally, it requires:
- [matplotlib](https://matplotlib.org/)
- [pandas](https://pandas.pydata.org/)
- [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/)
- [scikit-learn](https://scikit-learn.org/stable/index.html)
- [fbprophet](https://scikit-learn.org/stable/index.html)
- [hvplot](https://hvplot.holoviz.org/)  

See [installation](#installation) below for specifics.

---

## Installation

You will need Python 3.7, that supports for this application to run. An easy way to install python 3.7 is to download and install [Anaconda](https://www.anaconda.com/products/individual). After installing anaconda, open a terminal/command-prompt, and setup a python 3.7 environment, and then activate it like so:

```
# create an anaconda python 3.7 environment
# name can be any friendly name to refer to your environment, eg 'dev'
conda create --name dev python=3.7 anaconda

# activating the environment
conda activate dev

# use pip to install the above modules, eg:
pip install python-dotenv
...etc...
```


---

## Usage

The analysis is presented within a [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) notebook. To launch JupyterLab, from the root of this repo dirctory:

```
# within repo root 
$ jupyter lab
```
You can now open and run the notebook [credit_risk_resampling.ipynb](app/credit_risk_resampling.ipynb)  

---

## Contributors

[David Lopez](https://github.com/sububer)

---

## License

MIT