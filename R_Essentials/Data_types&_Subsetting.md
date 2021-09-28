#### Datatypes and R functions
- Assignment Operator:
X <- 11
print(x) Explicit Printing
x | its auto printing

- ## are used for adding comments
- R has 5 basic classes "atomic" of objects:
-Chracter ; numeric ; integer ; complex ; logical(boolean)
the most basic object in R is called a vector. And a vector can contain multiple copies of a single type of object. 
You can have a vector of characters or a vector of integers, one thing you cannot do with a standard vector is have mixed types of objects in a vector of characters and numerics, or numerics and integers, or integers and logicals. Everything in a vector has to be the same class.
You can have a list that's inside the list and one element of the list can be a data frame so, any element of the list can be anything. And that's actually why what makes list so useful.
- Numbers in R are generally treated as numeric objects 
- Nan represents none values
- R objects have attributes: names, dimensions, dimensions, class, length, other user defined attributes, Attributes are set using Attribute() function. The easiest way to create a vector is with the c()function, which stands for 'concatenate' or 'combine'.
#### Vectors and Lists
- c() function can be used to create vectors of objects, it can be used to create concatenation of intergers, boolean , complex and even chracters.The easiest way to create a vector is with the c()
| function, which stands for 'concatenate' or 'combine'.
- x <- vector(numeric, length =10) initialize vector with vaalue 10, default value is 0 for vector.
-  vector can have all data class, numeric and class.... you wont get error on mic=xing data types in vector but they will have their own style of display like (true, false, 2) will be like 1,0,2 as true signifies 1 in R
-  To convert classes in R, from numeric to chracter. numeric to boolean, we use the example: create a sequence of 0 to 6 x <- 0:6   >>  class(x) --- numeric   >> as.numeric(x) >> 0,1,2,3,4,5,6  >> as.logical(x) -- False True True True True.....  >> as.chracter(x) -- "0" "1" "2" "3" .....
- Lists are type of vector that contain elements of different classes;
x <- list(1, "a", TRUE, 1 + 4i)  >> x[[4]] ... we index elements with double brackets. o/p is 1 + 4i
-Matrices are vectors with n dimention attribute, nrow, ncol
m <- matrix(1: 6, nrow = 2, ncol = 3)
m >> first row element (1) is filled then column element (2) then row again column.

Binding rows and columns::
x<- 1:3
y<- 10:12
cbind(x,y)  
1,10  2,11  3,12 >> 1,2,3 are rows , 10 11 12 are columns
- Factor are vectors to represent Categorical data, Either Ordered or Unordered. A factor as an integer vector where each integer has a label. factors are treated specifically by modelling functions like lm() and glm(). factor has levels.
x<- factor(c("yes", "yes", "no", "yes"), levels = c("yes", "no")
x >> yes yes no no

- Missiing Values >> denoted by NA or NaN for undefined values.
is.na() >> used to test objects if they are NA || is.nan() to test nan. its also na value but converse in not true.
x <- c(1,2,3, NA,10)
is.na(x) >>> it returns True for NA values
- DATAFEAMES
-used to store tabular data, represented as special type of list where every element of list have same length, they can store different classes of objects in each column. Special attributes called row.names; they are created by read.table() or read.csv(). They are converted to matrix by data.matrix().
x<- data.frame(food = 1:5, bar + c(T,T,F,F))

- Other common arithmetic operators are `+`, `-`, `/`,
 and `^` (where x^2 means 'x squared'). To take the
 square root, use the sqrt() function and to take the
 absolute value, use the abs() function.


## SubSetting
There are number of operators that can be used to extract subsets of R objcts.
- [] always returns object of same class as original
- [[ ]] is used to extract elements of a list or a data frame. used to extract single element and class of returned object will not be list or data frame
- $ is used to extract elements of list, data frame by name, semantics are similar to hat of [[.

- Subsetting Lists:
- x <- list(foo = 1:4, bar = 0.6, baz = "hello") 
- x[1] >> 1,2,3,4
- x[[1]] >> 1 2 3 4
- x$bar >> 0.6
- x[["bar"]] >> 0.6
- $bar >> 0.6
- x[c(1,3)]  >> extracts $foo and $baz >>> 1234, hello

## Partial Matching
Partial matching of names is allowed with [[ and $.
whatever the name is of the list is if we use $ sign it does not find exact name and O/P result but in case of [[, we have to to specify full name else it will return NULL and if we cannot supply exact name, we have to add an attribute x[["a",Exact = False]]




