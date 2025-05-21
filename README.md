# main-flow-task-2
 import math

def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(math.sqrt(n)) + 1):
        if n % i == 0:
            return False
    return True

# Example usage:
n = int(input("Enter a number: "))
print("Prime:" if is_prime(n) else "Not Prime")