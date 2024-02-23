# Pandas Notes (For beginners by beginner)

## Outliers
Extreme values or unconsistent values are called outliers. It can be a very small or a very large e.g in voting system the age can be 2 years old or 900 years old, both are unconsistent.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/cb1683f9-df96-4732-9eec-dd9fa11c29c1">


## Data processing using pandas

### head()
The head() is used to display the first few rows of a DataFrame or a data structure containing tabular data. Optional parmeter can be given to head(param) for showing number of data to show.

### tail()
tail() function is used to view the last few rows of a DataFrame or a file. It's convenient to view last few rows without printing the whole table.

### shape()
It provides us the shape of DataFrame i.e the number of rows and columns for example DataFrame.shape() may give (10, 15). Here df has 10 rows and 15 columns.

### describe()
It gives the statistics of a DataFrame.
Here is a break down of statistics provided by the **describe()** function:
1) **Count:** The number of non-null values in each column.
2) **Mean:** The average value of each column.
3) **Standard Deviation(std):** The measure of amount of variations or dispersion in each column.
4) **Minumum(min):** The smallest value in each column.
5) **Maximum(max):** Largest value in each column.
6) **25th Percentile(25%):** Also known as the first quartile **(Q1)**, this represents the value below which 25% of the data falls.
7) **50th Percentile(50%):** Also known as the mdeian, this represents the value below which 50% of the data falls.
8) **75th Percentile(75%):** Also known as the third quartile **(Q3)**, this represents the value below which 75% of the data falls.

### iloc[position]
It provides the details of DataFrame at a specific location e.g details of Call of duty Ghost. id is provided for finding location.

### loc[position]
It provides the details of DataFrame at a specific location. index_key is provided for finding location. For example,
```python
df = pd.read_csv("vgsalesGlobale.csv", index_col="Name")
df.loc['Pokemon Red/Pokemon Blue']
```
Here Video game Name is the index key so in this case let's say loc["Pokemon Red/Pokemon Blue"], we get something like this:

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/78ebc1d7-e15b-4ba0-bcf9-5c51fa58341b">

These are the dataframe details about this row.

### corr()
Used to find correlation

To plot correlation
```
plt.figure(figsize=(10, 5))
correlation = df.corr()
sns.heatmap(correlation, cmap="BrBG", annot=True)
plt.show()
```
<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/ef871e87-d6ed-4271-a537-95a0f5bd9a5c">


### sort_values(by="feature")
Sort the dataframe on basis of feature. We can further add a prameter that will either sort the data in ascending order or not by default data is sorted in ascending order.
```
df.sort_values(by="feature", ascending=False).head()
```

### Drop duplicated rows
```
duplicate_rows_df = df[df.duplicated()]
```

### df["feature_name"].between(from, to)
Find data in between from - to
```
mid_2000 = df["Year"].between(2015, 2023)
```
