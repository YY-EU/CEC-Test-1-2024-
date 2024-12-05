# CEC-Test-1-2024-
CEC Test 1 2024 Preparations &amp; Exercises
#Q1: Loops and Iterations 
#Exercise 17 PYNative
#Find the sum of the series up to n terms.

#number of terms
n= 5

#first number of sequence
start =2
sum_seq =0

#run loop in n times
for i in range(0 , n):
    print(start, end= "+")
    sum_seq +=start

    #calculate the next term
    start = start*10 + 2

print("/nSum of above series is:" , sum_seq)

    
