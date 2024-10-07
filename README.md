# GUESS-THE-CUP-WITH-BALL
A ball is shuffled into three  cups.if three cups are given to you , you need to guess one cup which has the ball
from random import shuffle
def shuffle_this(cups):
    shuffle(cups)
    return cups
def guess_number():
    guess=''
    while guess not in ['0','1','2']:
        guess=input("enter a number between 0,1,2:- ")
    return int(guess)
def check_guess(cups,g):
    if cups[g]=='0':
        print("you guessed it")
        print(cups)
    else:
        print("better luck next time")
        print(cups)
l=['','0','']
shuffled_list=shuffle_this(cups)
g=guess_number()
check_guess(shuffled_list,g)
