- 👋 Hi, I’m @premkishorydv
    This code for advance calculator in language in python.

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b != 0:
        return a / b
    else:
        return "Error: Division by zero"

def modulo(a, b):
    if b != 0:
        return a % b
    else:
        return "Error: Division by zero"

def main():
    print("Welcome to the Advanced Calculator!")
    print("Available operations: +, -, *, /, %")

    while True:
        try:
            operation = input("Enter an operation (e.g., +, -, *, /, %): ")
            if operation.lower() == "exit":
                print("Thanks for using the calculator. Goodbye!")
                break

            num1 = float(input("Enter the first number: "))
            num2 = float(input("Enter the second number: "))

            if operation == "+":
                print("Result:", add(num1, num2))
            elif operation == "-":
                print("Result:", subtract(num1, num2))
            elif operation == "*":
                print("Result:", multiply(num1, num2))
            elif operation == "/":
                print("Result:", divide(num1, num2))
            elif operation == "%":
                print("Result:", modulo(num1, num2))
            else:
                print("Invalid operation. Please try again.")

        except ValueError:
            print("Invalid input. Please enter valid numbers.")

if __name__ == "__main__":
    main()
