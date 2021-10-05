# Missing Value
- Missing values play an important role in statistics and data analysis. Often, missing values must not be ignored, but rather they should be carefully studied to see if there's an underlying pattern or cause for their missingness.
- To make things a little more interesting, lets create a vector containing 1000 draws from a standard normal distribution with
- y <- rnorm(1000)
# Vectors+Data Frames
- These are tabular datatypes which means that they are used to store tabular data with rows and columns.
- The major diff is Matrices have only 1 class of data while data frames consist of many diff classes of data.
- we checkthe dimensions of the object using dim(variable_name) abd length using length(variable name).
- dim() allows to get or set the value for the my_vector eg. vector <- c(4,5) >> vector with 4 rows and 5 columns
- Using class() we get to data type. 
- ?matrix will give all the documentation.   
- we combine matrice and vectors using cbind or rbind function
# Data frames are used because matrices and vectors does not contain all kind of data numeric and chracter in an organised manner.
eg: A matrix of 4 rows and 5 columns with numbering from 1-20; binded usibg rorcbinf with chracter names causes problem for large data set therefore we need data frame.
- Data frame takes any number of arguments and returns single object of class "dataframe" thta is composed of original object!
- Make a data frame:
- data_values <- (1:20 , ncol = 5 , nrow = 4) >> This is forming a matrix
-  Row headings = patient names >> name <- c(abi, sbi, dbi, zbi)
-  dataframe <- data.frame(name,data_values)
-  Column_names = c(age, bp, weight, rating,test) 
-  colnames(dataframe) <- column-names
-  NOw dataframe is 4*5 dimension frame with Names as indexes and Age, bp weight etc as columns.
k
