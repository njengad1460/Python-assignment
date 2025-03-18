def calculator():
    try:
        num1 = float (input("Enter the first number: "))
        operation = input("enter the operation (+,-,*,/): ")
        num2 = float (input("Enter the second number: "))
        if operation == '+':
            resurts = num1 + num2
        elif operation == '-':
            resurts = num1 - num2
        elif operation == '*':
            resurts = num1 * num2
        elif operation == '/':
            if num2==0:
                print("Error:")
                return
            resurts = num1 / num2
        else:
            print("Invalid Operation")
            return
        print(f"Results : {num1} {operation} {num2} = {resurts}")
    except ValueError:
        print("invalid input")
        
calculator()
