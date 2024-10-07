#rock paper scissor game
#rock beats scissors
#scissors beats paper
#paper beats rock
import random
User_choice=int(input("Enter your choice: type 0 for rock,1 for paper,2 for scissor:"))
if User_choice>=3 or User_choice<0:
    print("you entered invalid number,you lost")
else:
    Computer_choice=random.randint(0,2)
    print("computer choose")
    print(Computer_choice)
    if Computer_choice==User_choice:
        print("Its a draw")
    elif Computer_choice==0 and User_choice==2:
        print("you lost")
    elif User_choice==0 and Computer_choice==2:
        print("you win") 
    elif Computer_choice> User_choice:      
        print("you lost")
    elif User_choice> Computer_choice :
        print("you win")           
