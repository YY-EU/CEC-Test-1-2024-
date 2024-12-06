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

#Q3 : If,else and elif statements (Week 4)
#isSquare Function
#Learn to Programme Python Textbook pg 110-111.

#Determine if two numbers represent a square.
#Function to determine if length and width represent a square.

def isSquare(length,width):

    if length == width:
        itsASquare = True
    else:
        itsASquare = False
    return itsASquare

#Test cases
result = isSquare(5,5)
if result:
    print('5 and 5 represent a square')
else:
    print('5 and 5 does not represent a square')

result = isSquare(9.5,10.5)
if result:
    print('9.5 and 10.5 represent a square')
else:
    print('9.5 and 10.5 does not represent a square')

#Get user input, convert to floats and call the function.
userLength = input('Enter a length: ')
userLength = float(userLength)
userWidth = input('Enter a width: ')
userWidth = float(userWidth)
if isSquare(userLength, userWidth):
    print(userLength, 'and', userWidth, 'represent a square.')
else:
    print(userLength, 'and', userWidth, 'does not represent a square.')

#Q4 Python Fucntions(Week 5)
#Exercise 6 PYNative
#Create a recursive function.

def addition(num):
    if num:
        #call same function by reducing number by 1.
        return num + addition(num-1)
    else:
        return 0

res = addition(10)
print(res)

#Q5 Python Functions(Week 5)
#Exercise 7 PYNative
#Assign a different name to function and call it through new name.

def display_student(name,age):
    print(name,age)

#Call using original name.
display_student("Emma", 26)

#Assign new name
showStudent = display_student

#Call using new name.
showStudent("Emma",26)

#Q6 If,else, elif statements (Week 4)
#A Grading Programme
#Learn to Programme Python Textbook pg 106.

#Convert a number score to a letter grade.
def letterGrade(score):
    if score >= 90:
        letter='A'
    elif score >= 80:
        letter= 'B'
    elif score >= 70:
        letter= 'C'
    elif score >= 60:
        letter= 'D'
    else:
        letter= 'F' #Fail through or default case
    return letter

grade1 = letterGrade(75)
print(grade1)
grade2 = letterGrade(82)
print(grade2)
grade3 = letterGrade(95)
print(grade3)

#Q6 Ossia

#Convert a number score to a letter grade.
def letterGrade(score):
    if score >=90:
        letter='A'
    elif score >=80:
        letter= 'B'
    elif score >=70:
        letter= 'C'
    elif score >=60:
        letter= 'D'
    else:
        letter= 'F' #Fail through or default case
    return letter

score= int(input('Enter a score: '))
grade= letterGrade(score)
print(grade)

#Q7 If,else, elif statements (Week 4)
#isEven function 
#Learn to Programme Python Textbook pg 113-114.

#Determine if a given integer is even or odd.

#Function to determine if the integer is even or odd.
def isEven(value):
    remainder = value%2
    if remainder ==0:
        return True
    else:
        return False

def EvenOrOdd(value):
    if isEven(value):
        print(value, 'is even.')
    else:
        print(value, 'is odd.')

userNumber = int(input('Enter a integer: '))
print(EvenOrOdd(userNumber))
                 
