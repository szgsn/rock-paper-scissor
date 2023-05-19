# rock-paper-scissor
Begginer Python Rock Paper Scissors Project
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇

import random


choose_by_person = input("What do you choose? Type 0 for Rock, 1 for Paper, 2 for Scissors. ")

if choose_by_person == "0":
  print(rock)
elif choose_by_person == "1":
  print(paper)
elif choose_by_person == "2":
  print(scissors)

print("Computer chooses: ")
choose_by_comp = random.randint(0,2)

if choose_by_comp == 0:
    print(rock)
elif choose_by_comp == 1:
  print(paper)
elif choose_by_comp == 2:
  print(scissors)


if choose_by_person == "0" and choose_by_comp == 2:
  print("You Win!")
elif choose_by_person == "0" and choose_by_comp == 0:
  print("Try again.")


if choose_by_person == "1" and choose_by_comp == 0:
  print ("You Win!")
elif choose_by_person == "1" and choose_by_comp == 1:
  print("Try again.")


if choose_by_person == "2" and choose_by_comp == 1:
  print("You Win!")
elif choose_by_person == "2" and choose_by_comp == 2:
  print("Try again.")

else:
  print("You lose.")
