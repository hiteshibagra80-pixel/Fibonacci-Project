# Fibonacci-Project
This Python program generates and displays the Fibonacci sequence up to a user-defined number of terms
# Python program to display the Fibonacci sequence

# Take input from the user
n = int(input("Enter the number of terms: "))

# First two terms
a, b = 0, 1
count = 0

# Check if the number of terms is valid
if n <= 0:
    print("Please enter a positive integer.")
elif n == 1:
    print("Fibonacci sequence up to", n, "term:")
    print(a)
else:
    print("Fibonacci sequence:")
    while count < n:
        print(a, end=" ")
        next_term = a + b
        a = b
        b = next_term
        count += 1
