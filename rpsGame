# Ask if user wants to play
# Ask user to select rock, paper or scissors. Returns a string.
# computer randomly chooses rock, paper, scissors
# check if there is a win. Return True if there is a win

import random

def choose_item() :
    
    player1_choice = ''
    player2_choice = random.choice(['R','P','S'])
    
    while not (player1_choice.upper() == 'R' or player1_choice.upper() == 'P' or player1_choice.upper() == 'S') :
    
        player1_choice = input('Choose either Rock, Paper or Scissors (R, P, S) :').upper()
        
    return (player1_choice,player2_choice)
 
 def check_win(p1_choice,p2_choice) :
    
    if p1_choice == 'R' and p2_choice == 'S':
        return True
    if p1_choice == 'S' and p2_choice == 'P' :
        return True
    if p1_choice == 'P' and p2_choice == 'R' :
        return True
    
    return False



player1_wins = 0
player2_wins = 0
draw_count = 0

while True :
    
    
    begin_game = input("Welcome to Rock, Paper, Scissors. Do you want to play? (y/n) :")
    
    if begin_game[0].upper() == 'Y':
            
        p1_choice, p2_choice = choose_item() # returns a tuple (p1, p2)

        print(f'Player 1 is has chosen {p1_choice}')
        print(f'Player 2 is has chosen {p2_choice}')


        if check_win(p1_choice,p2_choice):
            print ("Player 1 wins the game")
            player1_wins += 1
            print (f"Player 1 has won {player1_wins} times")
    

        elif check_win(p2_choice,p1_choice) :
            print ("Player 2 wins the game")
            player2_wins += 1
            print (f"Player 2 has won {player2_wins} times")
           

        else:
            print("its a draw")
            print (f"You have drawn {draw_count} times")
            
            
    else :
        break
