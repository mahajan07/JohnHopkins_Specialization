#### Reading Data
- read.table, read.csv for reading tabular data
specify name of file or db, header >> indicating file as header , sep >> strings indicating how columns are seperated, colClasses >> chracter vector indicating class of each column , nrows >> number of rows in dataset, skip >> number of lines to skip from beginning, stringAsFactors >> read strings as factors
- readLines, for reading lines a text file
- source, for reading in R code files(inverse of dump)
- dget, for reading in R code files( inverse of dput)
- load, for reading in saved workspaces
- unserialize, for reading single R objects in binary form

#### Writing Data
- write.table
- writeLines
- dump 
- dput
Dumping and dputing are useful because the resulting textual format is edit able and if corroupted, potentially recoverable. They preserve metadata.
- save
- serialize
- Texual data adhere to "Unix Philosophy". The format is not so space efficient.

## Data are read in using connection interfaces.
- file   >> opens a connection to a file
- gzfile >> open a connection to a file compressed with gzip
- bzfile >> opens a connection to a file compressed with bzip2
- url    >> opens a connection to a webpage
