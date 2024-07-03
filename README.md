import random

# Generate a random number between 1 and 10
number_to_guess = random.randint(1, 10)

# Ask the user to guess the number
print("I'm thinking of a number between 1 and 10.")
guess = int(input("Can you guess what it is? "))

# Keep asking until the user guesses correctly
while guess != number_to_guess:
    if guess < number_to_guess:
        print("Too low!")
    else:
        print("Too high!")
    guess = int(input("Try again: "))

print("Congratulations! You guessed the right number!")
