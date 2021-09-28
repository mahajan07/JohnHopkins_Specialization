- getwd() >> current working directory
- ls()  >> list all files
-  List all the files in your working directory using list.files() or dir().
-  Assign the value of the current working directory to a variable called "old.dir" >>  old.dir <-getwd()
-  Use dir.create() to create a directory in the current working directory called "testdir".
-   Create a file in your working directory called "mytest.R" using the file.create() function.
> file.create('mytest.r')  >> TRUE
> file.create('mytest.R') this is the format.
> file.info('mytest.R')
> file.exists('mytest.R')
> file.copy('mytest2.R', 'mytest3.R')
> file.remove('mytest.R')
