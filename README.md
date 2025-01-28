# pf-project

### Qurtulain
#### Roll No 156
###### Section BsAi 1C

### Summary of Data Cleaning and Analysis Steps

1. **Installed Required Libraries**:
    - Installed `pandas` for data manipulation.
    - Installed `seaborn` and `matplotlib` for data visualization.

2. **Imported Libraries**:
    - Imported `pandas` as `pd`.
    - Imported `seaborn` as `sns`.
    - Imported `matplotlib.pyplot` as `plt`.

3. **Loaded Data**:
    - Loaded the dataset from the file `IEA Global EV Data 2024.csv` into a DataFrame `df`.

4. **Exploratory Data Analysis**:
    - Checked the shape of the DataFrame using `df.shape`.
    - Displayed the first 4 rows using `df.head(4)`.
    - Displayed the last 4 rows using `df.tail(4)`.
    - Generated descriptive statistics using `df.describe()`.
    - Displayed DataFrame information using `df.info()`.
    - Checked for missing values using `df.isnull().sum()`.

5. **Data Cleaning**:
    - Removed rows with missing values using `df.dropna(inplace=True)`.
    - Renamed the column `Anie` to `Category` using `df.rename(columns={'Anie':'Category'}, inplace=True)`.

6. **Data Visualization**:
    - Plotted the count of each category using `sns.countplot(df['Category'])`.
    - Plotted a histogram of the `year` column with `unit` as hue using `sns.histplot(data=df, x='year', hue='unit', multiple='stack')` and displayed the plot using `plt.show()`.