The hard version scrambles the choices and presents them that way.

<!-- Import random function -->
import random

<!-- Define letters, numbers, and symbols -->
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']\
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']\
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

<!-- Define password -->
password = ""

<!-- Welcome print statement -->
print("Welcome to the PyPassword Generator!")

<!-- Inputs for letters, symbols, and numbers quantity -->
nr_letters = int(input("How many letters would you like in your password?\n"))
nr_symbols = int(input(f"How many symbols would you like?\n"))
nr_numbers = int(input(f"How many numbers would you like?\n"))

<!-- Takes user inputs and randomizes choices from each -->
for nr_letters in range(nr_letters):
    password += random.choice(letters)

for nr_symbols in range (nr_symbols):
    password += random.choice(symbols)

for nr_numbers in range(nr_numbers):
    password += random.choice(numbers)

<!-- Prints final password -->
print(password)
