# mario.py

import cs50

def main():
    print ("Height: ", end="") 
    height = cs50.get_int()
    
    if height > 23 or height < 0:
        print("Retry: ", end="")
        height = cs50.get_int()
    
    for i in range(height+1):
        print(' '*(height - i) + '#'*i + '  ' + '#'*i)
        
        
if __name__ == '__main__':
    main()
