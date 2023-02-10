SimpleCalculator


def add(x, y):
  return x + y

def subtract(x, y):
  return x - y 

def multiply(x, y):
    return x * y

def divide(x, y):
  return x / y

print("Please Select the Action:")
print("1. Addition")
print("2. Substraction")
print("3. Multiplication")
print("4. Division")

while True:
 
  choice = input("Enter your Choice(1/2/3/4: ")

  if choice in('1', '2', '3', '4'):
    num1 = float(input("Enter First Number: "))
    num2 = float(input("Enter Second Number: "))

    if choice == '1':
      print(num1, "+", num2, "=", add(num1, num2))

    elif choice == '2':
      print(num1, "-", num2, "=", subtract(num1, num2))

    elif choice == '3':
      print(num1, "*", num2, "=", multiply(num1, num2))

    elif choice == '4':
      print(num1, "/", num2, "=", divide(num1, num2))
      break

  else: 
      print("Wrong Entry!")

