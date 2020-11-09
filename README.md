# ANP Data Pipeline

This script intends to create an ETL pipeline for the ANP Fuel Sales repport.

## Goals

Extracting and Structuring data from the tables below:

- Sales of oil derivative fuels by UF and product
- Sales of diesel by UF and type

## Schema for the final data

| Column       | Type        |
| ------------ | ----------- |
| `year_month` | `date`      |
| `uf`         | `string`    |
| `product`    | `string`    |
| `unit`       | `string`    |
| `volume`     | `double`    |
| `created_at` | `timestamp` |

## Updates

### (MVP)
This is the first version of the script. It covers the following functions:
- Reading Excel data from selected sheet
- Defining columns' names
- Translating months' names from Portuguese to English
- Transforming each line of DataFrame to fit the schema of final data
- Loading this data to Spark and writing it in partitions

## Author
### Luciano Stoppa 
Profissional de "Data Engineering", | [Linkedin](www.linkedin.com/in/lucianostoppa)

##### O futuro é agora! | [www.ofuturoeagora.com.br](www.ofuturoeagora.com.br) 

###### São Paulo, 09/10/2020