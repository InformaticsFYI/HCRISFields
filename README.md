# HCRISFields

A helper file to identify fields in the Medicare Cost Reports

## Use

In Python, it can be loaded using the Pandas or Dask library:

```
dfFIELDS = df.read_csv('https://raw.githubusercontent.com/ohana-project/HCRISFields/master/fields.csv', dtype='str')
```

In R, it can be loaded using the RCurl library:

```
URL <- "https://raw.githubusercontent.com/ohana-project/HCRISFields/master/fields.csv"
Files <- getURL(URL)
Data <- read.csv(textConnection(Files))
```

## References

The majority of information in this file comes from a [SAS documentation file](https://www.cms.gov/Research-Statistics-Data-and-Systems/Downloadable-Public-Use-Files/Cost-Reports/Hospital-2010-form) found on the CMS website.  A number of fields are still not described, so this CSV file was produced for easier editing and use in scripts.

If you would like to contribute to this effort, feel free to submit a pull request!
