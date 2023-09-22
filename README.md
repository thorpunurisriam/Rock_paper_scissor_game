# Rock_paper_scissor_game
Rock Paper Scissor Game
import random
rock='''----------)(-------------)(-----------)'''
paper='''________________________)____________)___________)'''
scissor='''---------}-------------}-----------}'''
game_image=[rock,paper,scissor]
user_choice=int(input("Enter the Choice :Type 0 for Rock, 1 for the paper, 2 for the Sissor:"))
if user_choice>=3 or user_choice<0:
    print("You Entered an invalid Numbers[You Lost]")
else:
    print(game_image[user_choice])
    computer_choice=random.randint(0,2)
    print("Computer Choice:")
    print(game_image[computer_choice])
    if computer_choice==user_choice:
        print("it is A Draw Match")
    elif computer_choice==0 and user_choice==2:
        print("User Lose")
    elif user_choice==0 and computer_choice==2:
        print("User Win");
    elif computer_choice>user_choice:
        print("User lose")
    elif user_choice>computer_choice:
        print("User Win")
