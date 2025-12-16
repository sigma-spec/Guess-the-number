import random

secret_number = random.randint(1, 10)
attempts = 3
print("🎮 Guess the Number Game")
print("I chose a number from 1 to 10.")
print("You have 3 attempts.")

for attempt in range(1, attempts + 1):
    guess = int(input(f"Attempt {attempt}. Enter your number: "))
    if guess == secret_number:
        print("🔥 You guessed it! You win!")
        break
    else:
        if guess > secret_number:
            print("Too high!")
        else:
            print("Too low!")
else:
      print("❌ You lost. The number was:", secret_number)
