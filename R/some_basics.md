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
