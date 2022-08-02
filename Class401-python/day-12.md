# Reading 12 - Pandas
## 10 minutes to pandas
### Object Creation
* Creating a Series by passing a list of values, letting pandas create a default integer index
  * `s = pd.Series([1, 3, 5, np.nan, 6, 8])`
* Creating a DataFrame by passing a NumPy array, with a datetime index and labeled columns
  * `df = pd.date_range("20130101, periods=6)`
### Viewing Data
* How to view the top/bottom rows of the frame
  * df.head() - shows top 5
  * df.tail() - shows bottom 5
* Display the Index, columns
  * df.index
  * df.columns
* df.to_numpy() - finds the NumPy dtype that can hold all of the dtypes in the DataFrame
* df.describe() - shows a quick summary of your data
### Selection
* `df["A"]` - grabs data from the A column
* `df.loc[dates[0]]` - cross section data
* `df.loc[:, ["A", "B"]]` - multi axis data
