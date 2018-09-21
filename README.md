# Android_Session1_Assignment1.1
Assignment - 1  Session 1 – 
Introduction     Problem Statement  

1. Say True or False for the below statements: 
 • Prescriptive Analytics used to predict the future outcomes?  
 Ans:- TRUE 
 • Base R packages installed automatically? 
 Ans:- FALSE  

2. What is Recycling of elements in a vector?   
Ans:- R automatically recycles, or repeat, elements of the shorter vector. Recycling occurs when vector arithmetic is performed on multiple vectors of different sizes. R takes the shorter vector and repeats them until it becomes long enough to match the longer one. 
3. Give an example of recycling of elements. 
Ans:- 
> c(1,2,4)+c(6,0,9,10,13)
[1]  7  2 13 11 15
Warning message:
In c(1, 2, 4) + c(6, 0, 9, 10, 13) :
  longer object length is not a multiple of shorter object length
  
> c(1,2,4) + c(6,0,9,10,13)
[1] 7 2 13 11 15  As you can see, the c(1,2,4) vector repeated itself to form c(1,2,4,1,2) so that it could successfully match the previous term. If the shorter vector is not a vector of the longer one, then a warning message appears, but the operation still takes place. > c(1,2,4) + c(6,0,9,10,13) [1] 7 2 13 11 15   Warning message: In c(1, 2, 4) + c(6, 0, 9, 10, 13) :   longer object length is not a multiple of shorter object length.

Example-2:-
> x<-matrix(1:6,nrow = 3, ncol = 2)
> x
     [,1] [,2]
[1,]    1    4
[2,]    2    5
[3,]    3    6

Now we will add atwo element vector with this six element matrix
> x+c(1,2)
     [,1] [,2]
[1,]    2    6
[2,]    4    6
[3,]    4    8

Now the R has Recycled or Repeated the 2 elements shorter vector until it is long enough to match the longer one, six elements matrix as follow.
x+c(1,2,1,2,1,2)
