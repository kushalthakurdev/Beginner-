# Beginner-
so I am a student of engineering love to write code but I am weat at this soni want improve myself
import random

a = int(input("Enter your minimum range"))
b = int(input("Enter your maximum range"))
secret = random.randint(a, b)
attempt = int(input('No. of attempts you want'))

print("i am thinking a number. Can you guess it", attempt, "guesses??")
ch = 'yes'
while ch.lower() == "yes":
    for i in range(0, attempt):
        guess = int(input("Enter your guess number:"))
        if guess < secret:
            print("Get big higher")
        elif guess > secret:
            print("Get bit lower")
        elif guess == secret:
            print('correct guess')
            break

    ch = input('Do you want to try again(yes/no)?')
