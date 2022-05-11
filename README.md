# ETL_DB_Project-main
# Covid & Stock Market API :

A data pipeline is a set of tools and processes used to automate the movement and transformation of data between a source system and a target repository.

-   The data collection.
-   The organization of data.
-   Data transformation.
-   The transfer of this data to one or more systems.

![Timeline, waterfall chartDescription automatically generated](media/2f11a3362c603c14111880be13c6f066.png)

**Project Proposal :**

The purpose of this project Is to build and ETL that extract data from different sources and try to load them into our database , in our case two api (Alphavantage,covid)

the first one is Alphavantage api which provide us stock daily real time series data and other indicators, the second is covid Tracking api which provide us with daily corona virus data

The idea is to see if there is any correlation between daily cases of corona and the behaviour of the market and economic indicators

![What is ETL? - Databricks](media/f67136e5d03ae47c62d2b090f7594721.jpeg)

**Tools used :**

-   Python
    -   Pandas
    -   Requests
    -   SqlAlchemy
    -   Pymsql
-   MySql

# Extract :

![Définition de l&\#39;API REST: Qu&\#39;est-ce qu&\#39;une API REST (API RESTful)?](media/ffa6717b9f8418391b2e5aea21e4ec20.png)Thanks to request(python library) we can get our data from the api and get data (json format)

**Data Transformation:**

In the T part, First we transform our data from Json format to Dataframes

![](media/ed643ad220c589ffb586d0c0180862a7.png)

Then multiple operations like

-   Data cleaning
-   Data join
-   Data integration
-   Data filtering
-   Data deduplication
-   Data validation

III-Load :

In this last part we use SqlAlchemy to create a connection with our database and load the dataframes.

![](media/1843056a21474215e9dc783db78080bc.png)
