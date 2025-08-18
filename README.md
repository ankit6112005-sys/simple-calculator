# To create a simple calculator #
def addition(x,y):
    return(x+y)
def substract(x,y):
    return(x-y)
def multiplication(x,y):
    return(x*y)
def divide(x,y):
    return(x/y)

print("select operation: ")
print("1. Addition")
print("2. Substraction")
print("3. Multiplication")
print("4. Divide")

while True:
    choice=input("Enter choice: 1/2/3/4: ")
    if choice in('1','2','3','4'):
        num1=float(input("Enter the first number: "))
        num2=float(input("Enter the second number: "))
    if (choice == '1'):
        print(num1, "+", num2, "=", addition(num1, num2))

    elif (choice == '2'):
        print(num1, "-", num2, "=", substract(num1, num2))

    if (choice == '3'):
        print(num1, "*", num2, "=", multiplication(num1, num2)) 

    if (choice == '4'):
        print(num1, "/", num2, "=", divide(num1, num2))

    next_calculation = input("Let's do next calculation? (yes/no): ")
    if(next_calculation =="no"):
        print("Thank You ^^")
        break
    else:
        print("ok")
