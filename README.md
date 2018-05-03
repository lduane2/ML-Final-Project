# ML-Final-Project
Repository for the collaboration on our group's Machine Learning Final Project.

----
## Authors
* [Luke Duane](https://github.com/lduane2)
* [Michael McRoskey](https://github.com/michaelmcroskey)
* [Anthony Calvo](https://github.com/acalvo813)
* [Will Markley](https://github.com/willmarkley)


----
## Overview
Economic recessions and depressions are defined by the number of quarters U.S. GDP falls. Our project will analyze several macro-economic data sources to predict the GDP of the United States for a given quarter and subsequently predict whether a recession is likely. Our data sources include the [Bureau of Economic Analysis](https://www.bea.gov/), the [Bureau of Labor Statistics](https://www.bls.gov/), and [Congressional Budget Office](https://www.cbo.gov/). Our analysis is done in [iPython Jupyter Notebooks](https://ipython.org/notebook.html) using [Pandas](https://pandas.pydata.org/) and [TensorFlow](https://www.tensorflow.org/).

----
## Usage

We recommend using in a virtual environment such as [VirtualEnv](https://virtualenv.pypa.io/en/stable/)

```
# clone repository
git clone https://github.com/lduane2/ML-Final-Project.git
cd ML-Final-Project

# install dependencies (jupyter, tensorflow, pandas)
pip install -r requirement.txt

# run jupyter notebook
jupyter notebook

# navigate to dataCleaning.ipynb or basicModel.ipynb to view and execute code

```

---
## Data Files
1. data/
	* **`basicModel.ipynb`**: notebook to run basic model for Milestone 2
	* **`cleaned_econ_data.py`**: helper functions to import data into TensorFlow model
	* **`dataCleaning.ipynb`**: notebook to consolidate and clean data
	* **`description.txt`**: description of each data source
	* **`IncomeTaxRates.csv`**: high income tax bracket and low income tax bracket rate. *Source: [St. Louis Fed](https://fred.stlouisfed.org/graph/?id=IITTRHB,IITTRLB,)*
	* **`MonthlyFundsRate.csv`**: Effective federal funds rate by month. *Source: [St. Louis Fed](https://fred.stlouisfed.org/series/FEDFUNDS)*
	* **`MonthlyOilCPI.csv`**: oil prices. *Source: [St. Louis Fed](https://fred.stlouisfed.org/series/CUSRo0000SEHE)*
	* **`MonthlySNPInfo.csv`**: SNP real time price until 1970, broken down by month. *Source: [Yahoo Finance](https://finance.yahoo.com/quote/%5EGSPC/history?period1=18000&period2=1514782800&interval=1mo&filter=history&frequency=1mo)*
	* **`QuarterlyGDP.csv`**: quarterly GDP since 1940s
	* **`QuarterlyResults.csv`**: output of consolidated/cleaned data
	* **`QuarterlyUnemploymentSeasonallyAdjusted.csv`**: title, but only for ages 15-64. *Source: [St. Louis Fed](https://fred.stlouisfed.org/series/LRUN64TTUSQ156S)*
	* **`RealQuarterlyGDP.csv`**: real quarterly GDP since 1940s. Basically means it's adjusted for inflation. *Source: [St. Louis Fed](https://fred.stlouisfed.org/series/GDPC1)*
	* **`SP-Yearly.csv`**: inflation adjusted s&p data. *Source: [Multpl.com](http://www.multpl.com/inflation-adjusted-s-p-500/table/by-year)*
	* **`^GSPC.csv`**: S and P 500 closing data

---
## Resources
[Tensorflow Datasets](https://www.tensorflow.org/versions/master/get_started/datasets_quickstart)  
[Tensorflow DNNRegressor](https://www.tensorflow.org/api_docs/python/tf/estimator/DNNRegressor)  



