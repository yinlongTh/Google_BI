## Data Models and Pipelines

#### Data Model
: Show how data is organized and related to each other

#### Dimentional model
Fact - Dimention : Provide details for the Fact
And <strong>Attribute</strong> provides details for a Dimention

#### Schema 
is a output product after the modeling

- Star schema
![ADOdTP8WRAKHyHKl2QS14A_997c1cb1b57e40969848c1ee1b0275f1_Screen-Shot-2022-12-21-at-12 43 34-PM](https://github.com/yinlongTh/Google_BI/assets/108507768/dacbf2fc-6618-459a-a8e0-0930c3bbe8d4)

- Snowflake schema
![9EHB99ggRZ-jcYUuR7TCrw_6bf720e4e1484544bba3c40294ccedf1_Screen-Shot-2022-12-21-at-12 45 32-PM](https://github.com/yinlongTh/Google_BI/assets/108507768/bd8836d7-7784-4408-a257-3b1ec41642c6)

And others, Unstructured, Flat, Doc, Key-value etc.

#### Database types
- OLTP 
- OLAP
- Row-based
- columnar
- Distributed
- Single-homed
- Separated storage and compute | combined

#### Database choosing Consider
- Business needs
- Seize and type of data
- Data model

#### Data Marts & Data Warehouse & Data Lake

Data Lake
- DB that stores large amounts of raw data
- ELT normally
- Flat : data randomly store in the lake

Data Warehouse
- Someway organized data
- ETL normally
- hirrachy and files
- Data Mart : A subject-oriented database that can be a subset of a larger data warehouse

#### Database performance
1. Workload : Transaction, queries, etc.
2. Throughput : I/O speed of the hardware
3. Resources : Space and memory
4. Optimmization
5. Contention

#### Optimization Database
- Queries
- Indexes
- Data partitioning and clustering
<pre>
Create a table partitioned by an integer range (the years 2015 through 2022). Name it avocados_partitioned

CREATE TABLE
    `mydataset.avocados_partitioned`
PARTITION BY
    RANGE_BUCKET(Year, GENERATE_ARRAY(2015,2022,1))
AS (
    SELECT
        *
    FROM `mydataset.avocado_base`
);
</pre>

<pre>
Create a table partitioned by an integer range and clustered by type. Name it avocados_clustered.

CREATE TABLE
    `mydataset.avocados_clustered`
PARTITION BY
    RANGE_BUCKET(Year, GENERATE_ARRAY(2015,2022,1))
CLUSTER BY
    type
AS (
    SELECT
        *
    FROM `mydataset.avocado_base`
);
</pre>



















