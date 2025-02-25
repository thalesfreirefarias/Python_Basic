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
```
In the SQL query file, you should include what you're looking for, such as a filter, e.g., SELECT * FROM my_table WHERE condition. For the connection, you should use the SQL connection, like this:
```
connection = sqlite3.connect('my_database.db')
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
df.Types
```
###Summary Statistic
including:
mean, standard deviation, minimum, maximum, and percentiles for numerical columns.
```
df.Describe()
```
### Display Index, Columns, Data
general overview of the DataFrame, including:
Total number of entries (rows)
Column names
Number of non-null values in each column
Data types of each column
Memory usage

```
df.info()
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
