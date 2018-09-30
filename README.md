from math import sqrt
def sumDigits(number1,sign,number2):
    summ=number1+number2
    return summ
def subtraction(number1,sign,number2):
    subtraction=number1-number2
    return subtraction
def multiplication(number1,sign,number2):
    multiplication=number1*number2
    return multiplication
def factorial(number1,sign,number2):
    fact=1
    for i in range (1,number1+1):
        fact=fact*i
    return fact 
def power(number1,sign,number2):
    power=number1*number2
    return power
def division1(number1,sign,number2):
    if(number1>number2):
        division1=number1/number2
    else:
        division1=number2/number1
    return division1

def division2(number1,sign,number2):
    if(number1>number2):
        division2=number1//number2
    else:
        division2=number2//number1
    return division2
def division3(number1,sign,number2):
    if(number1>number2):
        division3=number1%number2
    else:
        division3=number2%number1
    return division3
def sqr(number1,sign,number2):
    sqr=sqrt(number1)
    return sqr
number1=int(input('Enter your first number: '))
sign=input('Enter "+"or"-"or"*"or"^"or"factorial"or"/"or"//"or"%"or"sqrt": ')
number2=int(input('Enter your second number: '))
if sign=='+':
    print(sumDigits(number1,sign,number2))
if sign=='-':
    print(subtraction(number1,sign,number2))
if sign=='*':
    print(multiplication(number1,sign,number2))
if sign=='factorial':
    print(factorial(number1,sign,number2))
if sign=='^':
    print(power(number1,sign,number2))
if sign=='/':
    print(division1(number1,sign,number2))
if sign=='//':
    print(division2(number1,sign,number2))
if sign=='%':
    print(division3(number1,sign,number2))
if sign=='sqrt':
    print(sqr(number1,sign,number2))
