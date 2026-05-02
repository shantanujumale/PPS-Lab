
#1Write a program to calculate the area of a circle and print the result as shown in the displayed 
test cases.
r = float(input("Enter the radius : "))
if 0.0<= r <=100.0:
	area = 3.14 * r * r
	print(f"Area of circle = {area:f}")
else:
	print("Enter a positive value upto 100")

#2  you are given a length L and breadth B and your task is to find the Area of the Rectangle.
L=int(input("L:"))
B=int(input("B:"))
area=L*B
print(f'{area}')

# Make use of the values of L and B read using the input function.

3#You are given a side S and your task is to find the Area of the square.

S=int(input("S:"))
a=S*S
print(f'{a}')
# Make use of the value of S read using the input function.


4#Write a Python program to print the area of a triangle.

b = float(input("Base: "))
h = float(input("Height: "))
area = 0.5 * b * h
print(f"Area: {area:.2f}")

5#Write a Python program to find the roots of a quadratic equation by taking the coefficients from the user.
import math
def find_roots(a,b,c):
	dis=b**2-4*a*c
	if dis>0:
		root1=(-b+math.sqrt(dis)) / (2 * a)
		root2=(-b-math.sqrt(dis)) / (2 * a)
		return root1,root2

	elif dis == 0:
		root1=-b/(2*a)
		return root1,
	else:
		real_part=-b/(2*a)
		imaginary_part=math.sqrt(abs(dis))/(2*a)
		root1=complex(real_part,imaginary_part)
		root2=complex(real_part,-imaginary_part)
		return root1,root2
a=float(input("a: "))
b=float(input("b: "))
c=float(input("c: "))
roots=find_roots(a,b,c)
if len(roots)==1:
	print(f"The root is: {roots[0]:.2f}")
elif len(roots)==2:
	print(f"The roots are: {roots[0]:.2f} and {roots[1]:.2f}")
else:
	print(f"The complex roots are: {roots[0]:.2f} and {roots[1]:.2f}")



6#Write a Python program to find the largest of three numbers.

n1 = float(input("Enter the first number: "))
n2 = float(input("Enter the second number: "))
n3 = float(input("Enter the third number: "))
if (n1>n2 and n1>n3):
	print(f"Largest number: {n1}")
elif (n2>n1 and n2>n3):
	print(f"Largest number: {n2}")
else:
	print(f"Largest number: {n3}")



7#Write a program to read temperature in Celsius and print the temperature in fahrenheit.

c=float(input("celsius: "))
f=(c*9/5)+32
print(f"fahrenheit: {f}")


8#write a Python program to perform union, intersection and difference operations on Set A and Set B.


a = list(map(int,input("Set A: ").split()))
A = set(a)
b = list(map(int,input("Set B: ").split()))
B = set(b)

# Write your code here to perform different operations
print("Union: ",A | B)
print("Intersection: ",A & B)
print("Difference: ",A - B)

9#Wrrite a Python program to check if a given year is a leap year or not.

y=int(input("Enter a year: "))
if(y%4==0):
	print(f"{y} is a leap year")
else:
	print(f"{y} is not a leap year")

10#Write a Python program to calculate the average marks for 5 subjects. The program should prompt the user to input the marks for each subject. After receiving the input, it should compute the average marks and then determine the corresponding grade based on the following grading system:

s1=float(input("subject 1: "))
s2=float(input("subject 2: "))
s3=float(input("subject 3: "))
s4=float(input("subject 4: "))
s5=float(input("subject 5: "))
total=s1+s2+s3+s4+s5
a=total/5
if a>=90:
	grade='A'
elif a>=80:
	grade='B'
elif a>=70:
	grade='C'
elif a>=60:
	grade="D"
else:
	grade="F"

print(f"Average Marks: {a:.2f}")
print(f"Grade: {grade}")

#11 Check whether the date is valid or not

from datetime import datetime,timedelta

def c(year,month,day):
	try:
		date=datetime(year,month,day)
		incremented_date=date + timedelta(days=1)
		return f"valid\nincremented date: {incremented_date.strftime('%Y-%m-%d')}"
	except ValueError:
		return "invalid"

year=int(input("year: "))
month=int(input("month: "))
day=int(input("day: "))

print(c(year,month,day))

12#Write a python program to print factorial of given number.

n=int(input("Enter a number : "))
fact =1
if n<0:
	print("Enter a positive number")
else:
	for i in range(1,n+1):
		fact=fact*i;
	print(f"Factorial of given number is : {fact}")

13#Write a Python program to print the following pattern.

num=int(input("Enter a number : "))
for i in range(num,0,-1):
	print("* "*i)

14# Combination of all the digits

vfrom itertools import permutations

def  com(d1,d2,d3):
	if 0<=d1<=9 and 0<=d2<=9 and 0<=d3<=9:
		c=permutations([d1,d2,d3])
		for item in c:
			print("".join(map(str,item)))
	else:
		print("Invalid")


d1=int (input("digit1 (0-9): "))
d2=int (input("digit2 (0-9): "))
d3=int (input("digit3 (0-9): "))

com(d1,d2,d3)

15#Write a Python program to perform multiplication of two matrices.

def matmult(A, B):
	# Write Code
	rowsA,rowsB=len(A),len(B)
	colsA,colsB=len(A[0]),len(B[0])
	if(colsA!=rowsB):
		print("Cannot multiply the two matrices. Incorrect dimensions.")
		return None
	result=[]
	for i in range(rowsA):
		row=[]
		for j in range(colsB):
			row.append(0)
		result.append(row)
	for i in range(rowsA):
		for j in range(colsB):
			for k in range(colsA):
				result[i][j]+=A[i][k]*B[k][j]
	return result

def readmatrix(name = ''):
	matrix=[]
	row=[]
	print(f"Enter values for {name}")
	m=int(input("Number of rows, m = "))
	n=int(input("Number of columns, n = "))
	for i in range(m):
		row=[]
		for j in range(n):
			row.append(int(input(F"Entry in row: {i+1} column: {j+1}\n")))
		matrix.append(row)
		row=[]
	return matrix
""" End of Function: matmult """



print("Matrix - A * Matrix- B =", matmult(matrixa, matrixb))


16# Prime number

def prime(num):
	if(num<=1):
		return False
	for i in range(2,int(num**0.5)+1):
		if num%i==0:
			return False
	return True

def pprime(n):
	for i in range(2,n):
		if prime(i):
			print(i)

n=int(input("Enter upper limit: "))
pprime(n)

17#rite a program to count the number of vowels using sets in a given string.

def vowel_count(str):
	count = 0
	vowel = set("aeiouAEIOU")
	for char in str:
		if char in vowel:
			count +=1
	print(count)
	# Write your code here to count the vowels
	
str = input()
vowel_count(str)

18#Write a Python program to find whether a given string is a palindrome or not.

w=input("")
if(w==w[::-1]):
	print("palindrome")
else:
	print("not a palindrome")

#19 remove puncuations

import string
def pun(s):
	table=str.maketrans('', '',string.punctuation)
	return s.translate(table)


s=input("")
print(pun(s))

20# Revere the string

w=input("")
rev=w[::-1]
print(f"{rev}")

21#Write a program to print the sum of digits of a number.

def sum(num):
	total=0
	while num>0:
		total += num%10
		num = num//10
	return total
num=int(input("num: "))
result=sum(num)
print(f"sum: {result}")

#22 sum of the digits of a number using recursion


def Sumof(n):
	if n==0:
		return 0
	return (n%10)+Sumof( n//10)

# take user input and add the function call
n=int(input())
print(Sumof(n))

#23  Phone book manager

# write your code...
phone_book={}
while True:
	print("1. Add Contact")
	print("2. Remove Contact")
	print("3. Display")
	print("4. Quit")
	choice=input("Enter choice (1-4): ")
	if choice == '1':
		name=input("Name: ")
		phone_number = input("Phone number: ")
		phone_book[name] = phone_number

	elif choice == '2':
		name=input("Name: ")
		if name in phone_book:
			del phone_book[name]
		else:
			print("Not found")

	elif choice=='3':
		print(phone_book)

	elif choice=='4':
		break
	else:
		print("Invalid")

#24Write a python program to define a module to find Fibonacci Numbers and import the module to another program

import fibonacci_module
try:
	n=int(input("Enter the max value: "))
	if n>0:
		seq=fibonacci_module.fibbo_seq(n)
		print("Fibonacci series upto",n,":")
		for num in seq:
			print(num, end= ' ')
	else:
		print("Please enter a positive integer")
except valueError:
	print("Invalid input")


#25 sum of the complaex number

class Complex ():
	def initComplex(self,num):
		print(f"complex number {num}")
		print("Real Part:",end=" ")
		self.real=int(input())
		print("Imaginary Part:",end=" ")
		self.imag=int(input())
	def display(self):
		print(f"{self.real}+{self.imag}i")
	def sum(self,c1,c2):
		self.real=c1.real+c2.real
		self.imag=c1.imag+c2.imag
c1 = Complex()
c2 = Complex()
c3 = Complex()
c1.initComplex(1)
c1.display()
c2.initComplex(2)
c2.display()
print("Sum:",end=" ")
c3.sum(c1,c2)
c3.display()


#26 display the car detail

class Car:
	# write your code here...
	def __init__(self,brand,price,model,color):
		self.brand=brand
		self.price=price
		self.model=model
		self.color=color
	def display(self):
		print(self.brand)
		print(self.price)
		print(self.model)
		print(self.color)
		



def get_car_details():
	brand = input("brand: ")
	price = float(input("price: "))
	model = input("model: ")
	color = input("color: ")
	return brand, price, model, color

print("Details for Car 1:")
car1_brand, car1_price, car1_model, car1_color = get_car_details()

# create an object car1
car1=Car(car1_brand,car1_price,car1_model,car1_color)

print("Details for Car 2:")
car2_brand, car2_price, car2_model, car2_color = get_car_details()

# Create the second car object
car2=Car(car2_brand,car2_price,car2_model,car2_color)

print("Car 1 Details:")
