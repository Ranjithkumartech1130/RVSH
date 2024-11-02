import random

def guessing_game():
    # Set the range for the random number
    lower_bound = 1
    upper_bound = 100
    random_number = random.randint(lower_bound, upper_bound)
    attempts = 0
    max_attempts = 10

    print(f"Welcome to the Guessing Game We are eagerly waitng for ur answer!")
    print(f"I'm thinking of a number between {lower_bound} and {upper_bound}.")
    print(f"You have {max_attempts} attempts to guess it.")

    while attempts < max_attempts:
        guess = input("What is in your mind: ")
        

        # Validate input
        if not guess.isdigit():
            print("you entered invalid number.")
            continue

        guess = int(guess)
        attempts += 1

        if guess < lower_bound or guess > upper_bound:
            print(f"Please guess a number within the range of {lower_bound} to {upper_bound}.")
        elif guess < random_number:
            print("Too low! Try again.")
        elif guess > random_number:
            print("Too high! Try again.")
        else:
            print(f"Congratulations! You've guessed the number {random_number} in {attempts} attempts.")
            break
    else:
        print(f"Sorry, you've used all your attempts. The number was {random_number}.")

# Run the game
guessing_game()