# Week 2 homework: pandas practice on the green taxi data

Use pandas to answer ten questions about the NYC green taxi trips of July 2026. Practise the syntax from the R-to-pandas map in Lab Brief 2.

## Set up

Create a notebook, `lab2_homework.ipynb`, in `submissions/`. Run this in the first cell:

```
import numpy as np
import pandas as pd

url = "https://d37ci6vzurychx.cloudfront.net/trip-data/green_tripdata_2026-07.parquet"
df = pd.read_parquet(url)
```

`read_parquet()` reads a parquet file the way `read_csv()` reads a CSV file. Week 3 explains parquet.

## Questions

Answer each question in its own cell. Start the cell with a comment such as `# Q1` and print the answer.

1. How many rows and columns does `df` have?
2. What is the type of each column, and how many missing values does each column hold?
3. List the distinct values of `payment_type` with the number of trips for each. Then convert the column to a category type and print its categories.
4. What are the mean and the median of `trip_distance`? Which is larger, and what does that suggest?
5. Show the row at position 10. Then show `fare_amount`, `tip_amount` and `total_amount` for the first three rows.
6. How many trips are longer than 10 miles?
7. How many trips were paid by credit card (`payment_type` 1) and carried two or more passengers?
8. Add a column `fare_per_mile` (`fare_amount` divided by `trip_distance`) for the trips with a distance above 0. What is its mean?
9. Add a column `long_trip` that is `"Yes"` when `trip_distance` is 5 miles or more and `"No"` otherwise. How many trips are `"Yes"`?
10. Find the mean of `passenger_count`, then the mean with missing values included (`skipna=False`). If they differ, explain why in a markdown cell.

## Submit

Run Restart and Run All, then save the notebook in `submissions/` before the week 3 lab.
