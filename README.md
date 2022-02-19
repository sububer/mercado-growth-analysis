# mercado-growth-analysis
FinTech Challenge 11 -- MercadoLibre Growth and TimeSeries Analysis  

See full implementation and notebook details in [forecasting_net_prophet.ipynb](app/forecasting_net_prophet.ipynb)  

---

## Overview Of Analysis

TBD

#### DataSet Details  

Data sets used to anlyze this space:
- [google_hourly_search_trends.csv](data/google_hourly_search_trends.csv) hourly google trend data
    - contains data: `Date | Search Trends `  
- [mercado_daily_revenue.csv](data/mercado_daily_revenue.csv)
    - contains data: `date | Daily Sales `  
- [mercado_stock_price.csv](data/mercado_stock_price.csv)
    - contains data: `date | close `  


## Results  

TBD  

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