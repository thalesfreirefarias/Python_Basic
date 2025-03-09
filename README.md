# Python_Basic
Basic commands to use in Python


# DailyStudy

![GitHub repo size](https://img.shields.io/github/repo-size/iuricode/README-template?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/iuricode/README-template?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/iuricode/README-template?style=for-the-badge)
![Bitbucket open issues](https://img.shields.io/bitbucket/issues/iuricode/README-template?style=for-the-badge)
![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/iuricode/README-template?style=for-the-badge)

### Day 1: Data loading:
- Read CSV FILE
  ```
  df=pd.read_csv('.csv')
  ```
-Read excel File
```
df= pd.read_excel('file.xlsx')
```
- Read SQL file
```
df=pd.read_sql('query_connection')
###In the SQL query file, you should include what you're looking for, such as a filter, e.g., SELECT * FROM my_table WHERE condition. For the connection, you should use the SQL connection, like this:
###connection = sqlite3.connect('my_database.db')
```

### Day 2 Data inspection
### Top Rows (Display)
```
df.head()
```
### Bottom Rows(Display)
```
df.tail()
```
### Data Types
```
df.dtypes
```

```
###Summary Statistic
including:
mean, standard deviation, minimum, maximum, and percentiles for numerical columns.
df.Describe()
```

```
df.info()
### Display Index, Columns, Data
general overview of the DataFrame, including:
Total number of entries (rows)
Column names
Number of non-null values in each column
Data types of each column
Memory usage
```

### Day 3 Data Cleaning

### Check for missing values
```
df.isnull().sum()
```
### fill Missing values
```
df.fillna(value)
```
### Drop Missing Values
```
df.dropna()
```
### Rename Columns
```
df.rename(columns ={'old_name': 'new_name'})
```
### Drop Column
```
df.drop(columns=['columns_name'])
```

### Day 4 Data Transformation

```
### Applies a function to each value in the "column"
df['column'].apply(lambda:function(x))
df = pd.DataFrame({'column': [1, 2, 3, 4]})
df['new_column'] = df['column'].apply(lambda x: x * 2)
```

```
### Groupby and Aggegate
df.groupby('column').agg({'column':'sum'})
```

```
###Pivot tables- > Calculates the mean of columns2 for each unique value in columns1.
df.pivot_table(index='columns1'.values='columns2'.aggfunc='mean')
result = df.pivot_table(index='category', values='values', aggfunc='mean')
```

```
### Merge Dataframes -> Function combines two DataFrames (df1 and df2) based on a common column.
pd.merge(df1,df2, on = 'column')

df1 = pd.DataFrame({'column': [1, 2, 3], 'values1': ['A', 'B', 'C']})
df2 = pd.DataFrame({'column': [2, 3, 4], 'values2': ['X', 'Y', 'Z']})

result = pd.merge(df1, df2, on='column')

## excludes 1 and 4 because don't have a common column
```

```
###Concateate Dataframes
pd.concat([df1,df2])

result = pd.merge(df1, df2, on='customer_id', how='left')
how-> inner( just with values), outer(fill when NaN,right
```

### Day 5 Data Transformation

```
###Histogram
df['column'].hist()
or
import matplotlib.pyplot as plt

df['column'].hist(bins=20, edgecolor='black')
plt.xlabel('Valores')
plt.ylabel('Frequência')
plt.title('Histograma da coluna')
plt.show()
```

```
###boxplot
df.boxplot(column=['column1', 'column2'])
```

```
###Scatter plot
df.plot.scatter(x='col1', y='col2')
```

```
###Line plot
df = pd.DataFrame(data)
df.plot.line()
plt.title('Gráfico de Linhas de Exemplo')
plt.xlabel('Índice')
plt.ylabel('Valores')
plot.show()
```

```
###Bar chart
df['column'].value.counts().plot.bar()
df['column'].value_counts().plot(kind='bar', color='skyblue', edgecolor='black')
```

### Day 6 Statistical Analysis
```
###correlation Matrix
df.corr()
```

```
###covariance matrix
df.cov()
```

```
###Value counts
df['column'}.value_counts()
```

```
df['column'].unique()
```

```
df['column'].nunique()
```

### Adjustments and improvements.

The project is still under development, and the upcoming updates will focus on the following tasks:

- [x] Advanced courses about Phyton

The following tools were used in the construction of the project:

- [Python](<https://www.python.org/doc//>)



## 🤝 Creator

<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="grecia.jpg" width="100" alt="Foto do Thales Farias no GitHub"/><br>
        <sub>
          <b><a href="https://www.linkedin.com/in/thalesfreirefarias/" target="_blank">Thales Farias</b>
        </sub>
      </a>
    </td>
  </tr>
</table>
