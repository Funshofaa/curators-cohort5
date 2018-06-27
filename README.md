# curators-cohort5
Basic coding project
import random

def welcome():
    name_user = raw_input('Enter your id')
    print('welcome to guess game', name_user)
    
    
def game():
    num = random.randint(1, 20)
    for i in range(4):    
        user_ans = int(raw_input('enter the number'))    
        if user_ans < num:
           print('your guess is lower')    
        elif user_ans > num:
           print('your guess is higher')    
        else:
            print ('good job')
        
def main():
    welcome()
    game()
    
main()
