# two-a-
def fn(n):
    if n <= 1:
        return n
    else:
        return fn(n-1) + fn(n-2)

try:
    num = int(input("Enter a number: "))
    if num >= 0:
        print(f'fn({num}) = {fn(num)}')
    else:
        print("Input should be greater than or equal to 0")
except ValueError:
    print("Try with numeric value")

# two-b-
def bin2Dec(val):
    return int(val, 2)

def oct2Hex(val):
    return hex(int(val, 8))

try:
    num1 = input("Enter a binary number: ")
    print(bin2Dec(num1))
except ValueError:
    print("Invalid literal in input with base 2")

try:
    num2 = input("Enter an octal number: ")
    print(oct2Hex(num2))
except ValueError:
    print("Invalid literal in input with base 8")
    
