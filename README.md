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

#Q2: Loops and Iterations
#Exercise 11 PYNative
#Print all prime numbers within a range.

start = 25
end = 50
print("Prime numbers between", start, "and", end, "are:")

for num in range(start, end + 1):
    # all prime numbers are greater than 1
    # if number is less than or equal to 1, it is not prime
    if num > 1:
        for i in range(2, num):
            # check for factors
            if (num % i) == 0:
                # not a prime number so break inner loop and
                # look for next number
                break
        else:
            print(num)
