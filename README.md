
# Rock Paper Scissors
In this project I have created a small game of rock paper and scissors


## Usage

```python
import random
print("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors")
num = int(input())
rannum = random.randint(0,2)

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

if num == 0:
  print(rock)
elif num == 1:
  print(paper)
elif num == 2:
  print(scissors)
else:
  print("you have input wrong number")

print("computer chose:")
if rannum == 0:
  print(rock)
elif rannum == 1:
  print(paper)
else:
  print(scissors)
if num == 0 and rannum == 0:
  print("Draw")
elif num == 0 and rannum == 1:
  print("You lose")
elif num == 0 and rannum == 2:
  print("You Win")
elif num == 1 and rannum == 0:
  print("You Win")
elif num == 1 and rannum == 1:
  print("Draw")
elif num == 1 and rannum == 2:
  print("You Lose")
elif num == 2 and rannum == 0:
  print("You Lose")
elif num == 2 and rannum == 1:
  print("You Win")
elif num == 2 and rannum == 2:
  print("Draw")
else:
  print("This repl has exited Run again ?")
  
