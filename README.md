# CFU10.py
import random

# Start of the program
random_number = random.randint(1, 10)  # Generate a random number between 1 and 10
attempts = 0  # Initialize attempts = 0

while True:
    guess = int(input("Guess a number between 1 and 10: "))  # Prompt user for a guess
    attempts += 1  # Increase attempts by 1

    if guess == random_number:  # Is the guess equal to the random number?
        print(f"Correct! It took you {attempts} attempts.")  # Print number of attempts taken
        break
    else:
        if guess > random_number:  # Is the guess too high?
            print("Too High")  # Inform the player their guess is too high
        else:
            print("Too Low")  # Inform the player their guess is too low
