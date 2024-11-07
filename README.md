operation = input("Enter your operation : ")
n = int(input("Enter the count of your numbers: "))
list_numbers = []
while len(list_numbers) < n:
    b = float(input("Enter your number: "))
    list_numbers.append(b)
result = list_numbers[0]
for i in list_numbers[1:]:
    if operation == "+":
        result += i
    elif operation == "-":
        result -= i
    elif operation == "*":
        result *= i
    elif operation == "/":
        if i != 0:
            result /= i
        else:
            print("tarif nashode")
            break
print("Result:", result)
