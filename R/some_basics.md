## Printing some thing
**You can print multiple items in one print function**
```r
name <- 'ismail'
print('my name is ', name)
```
**You will get an error like this**
```
ERROR!
Error in print.default("my name is ", name) : 
  invalid printing digits -2147483648
Calls: print -> print.default
In addition: Warning message:
In print.default("my name is ", name) : NAs introduced by coercion
Execution halted
```
**we use ```cat``` function to solve that issue**
```r
cat('my name is ', name)
```
**Output**
```
my name is  ismail
```
**keep in mind ```cat``` can't print compound data structures such us matrix and lists**
## sequances
```r
a <- 1:5 # [1] 1 2 3 4 5
b <- seq(from = 0, to = 5, by = 2) # [1] 0 2 4
# sequences with fractional increment, create sequances based on length.output value !
d <- seq(from = 1.0, to = 2, length.out = 6) # [1] 1.0 1.2 1.4 1.6 1.8 2.0
# repeat number as many as you like
c <- rep(2, times = 6) # [1] 2 2 2 2 2 2
```
## comparisons in R
```r
==     #equal
=!     #not equal
<      #less than
>      #greater than
<=     #less than or equal to
>=     #greater than or qual to 
```
```r
x <- c(1, 2, 3, 4, 5)
any(x == 4)      #True
all(x == 1:5)    #True
```
## Selecting vector elements
```r
x <- c(1:10)
x[1]        # position 1 = 1
x[4]        # Position 4 = 4
x[7:11]     # [1]  7  8  9 10 NA
x[c(1,5,6)] # position 1 5 and  6 = [1] 1 5 6
x[-5]       # Ignore 5th position and return all other values = [1]  1  2  3  4  6  7  8  9 10
x[-(1:6)    # ignore 1 up to 6th position and return other values = [1]  7  8  9 10
x <= 5      #[1]  TRUE  TRUE  TRUE  TRUE  TRUE FALSE FALSE FALSE FALSE FALSE
x[x <= 6]   # [1] 1 2 3 4 5 6
```
