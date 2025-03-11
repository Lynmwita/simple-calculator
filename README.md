#simple calculator program

#function to perform the chosen mathematical operation
def calculate(num1, num2, operation):
    if operation == '+' :
        return num1 + num2
    elif operation == '-' :
        return num1 - num2
    elif operation == '*' :
        return num1 * num2
    elif operation == '/' :
        return num1 / num2
    else:
        return "invalid operation"
    

#function to get the input from the user
def get_input():
    num1 = float(input("Enter the first number:"))
    num2 = float(input("Enter the second number:"))
    operation = input("Enter the operation (+, -, *, ): ")
                      
#perform the calculation
    result = calculate(num1, num2, operation)
    
#print the result
    print(f"The result of {num1} {operation} {num2} = {result}")
    
