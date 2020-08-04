# Three-cup-monte
#initial_list

my_list=['','O','']

#shuffle_list

def shuffle_list(my_list):
    shuffle(my_list)
    return my_list
    
#user_guess
    
  def player_guess():
    guess=''
    while guess not in ['0','1','2']:
        guess=input("Pick a number 0,1 or 2")
    return int(guess)
    
   #checking the guess
    
   def check_guess(my_list,guess):
    if my_list[guess]=='O':
        print("Correct")
    else:
        print("Wrong answer")
        print(my_list)
        
#initial list
my_list=['','','O']
#shuffle list
mixedup_list=shuffle_list(my_list)
#user guess
guess=player_guess()
#check the list
check_guess(my_list,guess)
