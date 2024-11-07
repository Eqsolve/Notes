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
