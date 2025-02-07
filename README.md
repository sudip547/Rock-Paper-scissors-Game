import random

def play ():
    user=input(" 'r' for rock,'p' for paper,'s' for scissors \n")
    computer=random.choice(['r','p','s'])

    if user==computer:
        return 'tie'
    
    if win(user,computer):
        return 'You Win'
    return 'You Lost'
def win(player,opponent):

    if(player=='r' and opponent=='s') or (player=='s' and opponent=='p') or (player=='p'and opponent=='r'):
        return True
    
print(play())

