# IF Else Conditions
if(condition(x >3)) {
    do something y <- 10 or write only 10
 } else {
      do something else y <- 0 or only 0
 }
 
 - If , else if, else
 if (condition) {
        do something
  } else if (condition) {
  do something different
 } else { 
      do something different }

# For Loop
for (i in 1 : 10) {
        print(x[i])
   }
 x <- c('a', 'b','c', 'd')
 - for (i in 1:4) 
 {      print(x[i])
 }
 - for i in seq_along(x)
    { print(x[i])
    }
  - for (letter in x)
  {   print(letter)  }
  - NESTED FOR LOOPS
  - for (i in seq_len(nrow(x)))
    {       for (j in seq_len(ncol(x)))
           {  print(x[i,j])  }
           }

# While
count <- 0
while (count < 10) {
        print(count)
        count <- count +1 }
- Begin with testing a condition, if true , they execute loop body. Once loop is executed , condition is tested again & so on.
- If not written properly, may be turn into infinite loop
- Check various conditions using operators


# Repeat
- It initiates an infinite loop & has statistical applications. Only way to stop loop is BREAK
x0 <- 1
tolerence <- le-8

repeat {
        x1 <- computeEstimate()
        if (abs(x1 - x0) < tolerence)
        { 
        break
        }
        else 
        {
        x0 <- x1
        }
      }

# Break


# Next & Return
- Skip iterations we use next:
 for (i in 1:100) {
        if (i <= 20)
        { # skip Iteration
        next
        }
        ## do something here
      }
   -return signals that a function should exit and return a given value

# Functions


# R Binds


# Lexical Scoping


# Dynamic Scoping


# Data / Time
