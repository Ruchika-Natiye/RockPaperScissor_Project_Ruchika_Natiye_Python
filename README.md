# RockPaperScissor_Python_Project_Ruchika_Natiye
This is a basic beginner level python project using conditional nested if elif-else statements.This is very easy and an interesting game that we used to play during our schooldays.Here,rock wins against scissor, scissor wins against paper and paper wins against rock!

CODE: 

import random
user_choice=int(input("Enter your choice:\nType 0 for Rock\nType 1 for Paper\nType 2 for Scissor"))
if user_choice==0:
    print("user chose Rock!")
elif user_choice==1:
    print("user chose Paper!")
elif user_choice==2:
    print("user chose Scissor!")
    
if user_choice>=3 or user_choice<0:
    print("You entered invalid number\nYou Lose!:(")

else:
    computer_choice=random.randint(0,2)
    if computer_choice==0:
        print("computer chose Rock!")
    elif computer_choice==1:
        print("computer chose Paper!")
    elif computer_choice==2:
        print("computer chose Scissor!")
if computer_choice==user_choice:
    print("It's a draw!")
elif computer_choice==0 and user_choice==2:
    print("You lose!")
elif user_choice==0 and computer_choice==2:
    print("You win!")
elif computer_choice>user_choice:
    print("You lose!")
elif user_choice>computer_choice:
    print("You win!")
