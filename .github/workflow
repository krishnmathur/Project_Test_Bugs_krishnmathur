def add_strings(num1, num2):
    if num1 == "" and num2 == "":
        return "0"
    
    # Rest of the code remains the same as before
    len1 = len(num1)
    len2 = len(num2)
    max_len = max(len1, len2)
    num1 = num1.zfill(max_len)
    num2 = num2.zfill(max_len)
    carry = 0
    result = []
    
    for i in range(max_len - 1, -1, -1):
        digit_sum = int(num1[i]) + int(num2[i]) + carry
        carry = digit_sum // 10
        digit_sum %= 10
        result.insert(0, str(digit_sum))
    
    if carry > 0:
        result.insert(0, str(carry))
    
    result_str = ''.join(result)
    
    return result_str

# Example usage
num1_str = input("Enter the first number: ")
num2_str = input("Enter the second number: ")

result_str = add_strings(num1_str, num2_str)
print("The sum is: " + result_str)
