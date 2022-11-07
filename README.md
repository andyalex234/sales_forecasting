# Pharmaceutical Sales Prediction across multiple stores
![image](https://user-images.githubusercontent.com/59474650/200432138-f1c388f1-d0c0-4371-8ae2-9bdf92ed84ea.png)


**Table of Content**
* [Project Overview](#project-overview)
* [Data and Features](#data-and-features)
* [Installation Guide](#installation-guide)
* [Project Structure](#project-structure)
* [LICENCE](#licence)
* [Contributers](#contributors)
* [Acknowledgement](#acknowledgement)

## Project Overview
You work at Rossmann Pharmaceuticals as a Machine Learning Engineer. The finance team wants to forecast sales in all their stores across several cities six weeks ahead of time. Managers in individual stores rely on their years of experience as well as their personal judgment to forecast sales. 

The data team identified factors such as promotions, competition, school and state holidays, seasonality, and locality as necessary for predicting the sales across the various stores.

Your job is to build and serve an end-to-end product that delivers this prediction to analysts in the finance team. 

## Data and Features 
Most of the fields are self-explanatory. The following are descriptions for those that aren't.


| Data fields         | Description |    
|---------------------|:------------
| Id                  |   an Id that represents a (Store, Date) duple within the test set | 
| Store               |    a unique Id for each store                                     |   
| Sales               |  the turnover for any given day (this is what you are predicting)|   
| Customers           | the number of customers on a given day |   
| Open                | an indicator for whether the store was open: 0 = closed, 1 = open |   
| StateHoliday        | indicates a state holiday. Normally all stores, with few exceptions, are closed on state                         holidays. Note that all schools are closed on public holidays and weekends. a = public                            holiday, b = Easter holiday, c = Christmas, 0 = None|   
| SchoolHoliday       | indicates if the (Store, Date) was affected by the closure of public schools|   
| StoreType           | differentiates between 4 different store models: a, b, c, d |   
| Assortment          | describes an assortment level: a = basic, b = extra, c = extended. Read more about                                assortment here|   
| CompetitionDistance | the distance in meters to the nearest competitor store |   
| CompetitionOpenSince[Month/Year]| gives the approximate year and month of the time the nearest competitor has                            opened |   
| Promo           |indicates whether a store is running a promo on that day|   
| Promo2          | Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not                                 participating, 1 = store is participating |   
| Promo2Since[Year/Week]| describes the year and calendar week when the store started participating in Promo2|   
| PromoInterval|describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store| 



## Installation Guide
```
git clone https://github.com/andyalex234/sales_forecasting.git
cd sales_forecasting
pip install -r requirements.txt
```

## Project Structure
- `Notebooks` - Contains the EDA, preporcessor
- `Models` - Conatins machine learning models
- `Scripts` - Contains modules that are used in the Notebooks and some utility functions as well
- `Data' - Conatains the csv or `.dvc.csv` file that we're going to use in this project
- `test` - Contains the unit and integrations tests of the project

## LICENCE
 MIT

## Contributors

<a href = "https:/r/github.com/andyalex234">
  <img src="https://contrib.rocks/image?repo=andyalex234/logistic-optimization" />
  Andenet Alexander
</a>

> any type of contribution is welcomed. [Fork](https://github.com/andyalex234/fund-by-gps-location/fork), apply your changes and make a [pull request](https://github.com/andyalex234/fund-by-gps-location/pull).

## Acknowledgement
This project was given as a challange by [10Academy](https://www.10academy.org/) for the trainees.
