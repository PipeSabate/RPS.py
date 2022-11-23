#Utilizamos import random para acceder a la herramienta de seleción aleatoria


import random
ask = 'y'
ask= input('you want to play  (y)es or (n)o? ' ,  )
while ask == "y":
        
        print("let´s go")
        print('(r) for Rock , (p) for paper  and (s) for Scissors')
        letter = input ('Chose a letter   '   ,      )
        if letter == 'r':
            print('You Choose Rock')
        elif letter == 's' :
            print('You Choose Scissors')
        elif letter == 'p':
            print ('You Choose Paper')
        else  :
            print('invalid option , try again')
        rpr = ['r' , 'p' , 's']
        pc = random.choice(rpr)
        if  pc == 'r':
            print('Y choose Rock')
        elif pc == 's' :
            print('Y choose Scissors')
        elif pc == 'p':
            print ('Y choose Paper')

        if pc == letter :
            print ('Empatamos')
        if pc == 'r' and letter == 'p':
            print ('You Win!')
        if pc == 'r' and letter == 's': 
            print(' I WIN , U LOSE')
        if pc == 'p' and letter == 's':
             print ('You Win!')
        if pc == 'p' and letter == 'r':
            print('I WIN , U LOSE')
        if pc == 's' and letter == 'r':
             print ('You Win!')
        if pc == 's' and letter == 'p':
            print('I WIN , U LOSE')
        ask= input('you want to play again  (y)es or (n)o? ' ,  )
        continue
        
print('El juego a terminado')
