## keywords note
- **C** : combine function, used to combine values.
- **vecotr** : sequance of data values or just an array but you can't store diffrent data structure in 1 variable
## list and remove
```r
x <- 'abcd'
g <- 23
l <- 'S'
h <- 'a24'
ls() # [1] "g" "h" "l" "x"
rm(h) # object 'h' not found
rm(list=ls())
ls() # character(0)
```
## variable structure
```r
x <- 2  #  num 2
name <- 'ismail'  # chr "ismail"
valid <- TRUE  # logi TRUE
```
**You can view all variable structure at once**
```r
ls.str()   #name :  chr "ismail"
           #valid :  logi TRUE
           #x :  num 2
```
**variables start with dot are hiden you can't see it with ```list variables```**
```r
name <- 'ismail'  
.hoppy <- 'hiden'
ls()              # [1] "name"
ls(all.names = TRUE)  # [1] ".hoppy" "name"
```
**You can con mutlitble varaibles in one var using combine ```C```but be sure both variable have same data structure**
```r
a1 <- c(1, 2, 3)           # num
a2 <- c('a', 'b', 'c')     # chr
a3 <- c(a1, a2)            # chr
ls.str()
```
