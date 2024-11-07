## list and remove
```r
x <- 'abcd'
g <- 23
l <- 'S'
h <- 'a24'
ls() # [1] "g" "h" "l" "x"
rm(list=ls())
ls() # character(0)
```
