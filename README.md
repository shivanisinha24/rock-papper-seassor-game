# rock-papper-seassor-game
import random
computer= random.choice([-1,0,1])
youstr = input ("Enter your choice: ")
youDict = {"r": 1, "p": -1, "s": 0}
reverseDict = {1: "rock", -1:"papper", 0:"seassor"}

you = youDict[youstr]

print(f"You chose {reverseDict[you]}\n Computer chose {reverseDict[computer]}")

if(computer == you):
    print("its a draw")

else:
if((computer - you)== -1 or (computer - you) == 2):
  print("You lose")
else:
  print("you win!")
