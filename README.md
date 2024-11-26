# Count-Potent-Number

Let’s define a positive integer as “potent” if it contains only one non-zero digit. For instance, numbers like 5000, 4, 1, 10, and 200 are considered potent, while numbers like 42, 13, 666, 77, and 101 are not. Given an integer n, your task is to count how many potent numbers x exist such that 1 ≤ x ≤ n.

def count_potent_numbers(n):

    count = 0
    for d in range(1, 10):  # d = 1 to 9
        num = d
        while num <= n:  # Generate numbers by multiplying by 10
            count += 1
            num *= 10
    return count

# Input and Output
n = int(input())  # Read the integer n
print(count_potent_numbers(n))

