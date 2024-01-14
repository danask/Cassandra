# Cassandra
Data modeling with Cassandra
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

In this project I will create an Apache Cassandra database which can create queries on song play data to answer the questions.

## Datasets
The dataset event_data is stored in the directory event_data which contains CSV files partioned by date. Here are examples of filepaths to two files in the dataset:

- event_data/2018-11-08-events.csv
- event_data/2018-11-09-events.csv
  
## ETL pipeline

![image](https://github.com/danask/Cassandra/assets/23080044/0a7215d6-eed0-48da-bfa9-b3d9fd15ecfc)


The figure above presents the ETL pipeline of project. It consists of three steps:

1. Extract: Process CSV files in the directory event_data to create a new CSV file.
2. Transform: Create an Apache Cassandra database and transform data from the new CSV file into tables.
3. Load: Do queries on database.
