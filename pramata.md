#Problem 1
Yet Another Xor Problem

You are given an array A of size N and an integer K. You need to find the value of :
![(cnt1+cnt2)^2+(cnt2+cnt3)^2+(cnt3+cnt1)^2-(cnt1^2+cnt2^2+cnt3^2)](https://latex.codecogs.com/gif.latex?(cnt1&plus;cnt2)^2&plus;(cnt2&plus;cnt3)^2&plus;(cnt3&plus;cnt1)^2-(cnt1^2&plus;cnt2^2&plus;cnt3^2))

,where

cnt1 : Number of subsets of array having cumulative xor less than K.

cnt2 : Number of subsets of array having cumulative xor equal to K.

cnt3 : Number of subsets of array having cumulative xor greater than K.

 

Input Format :

The first line contains an integer T denoting the number of test cases.

First 2 lines of each test case has 2 integers N and K respectively.

Next line has N integers denoting the array A.

Output Format :

Print answer for each test case under modulo 
in a new line.
