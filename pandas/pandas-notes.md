# Loading data

```python
df = pd.read_csv('data.csv')
```

# Plotting a histogram

To plot a histogram of a specific feature (i.e. column), just index into
that column using the DataFrame's default indexing method and call .hist():

```python
df['some_col'].hist()
```
Calling .hist() on a DataFrame *without* indexing into a specific column
creates histograms for every column in the DataFrame.

When plotting a histogram  *with* a PDF, you need to used the argument
`normed=1`. Otherwise, the histogram will be on an entirely different scale
than the PDF.
