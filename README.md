# ATM_Project_Python
ATM_Code
name = input("What is your name? \n")
allowedUsers = ['Jerry','Angela','Love']
allowPassword =['passwordJerry','passwordAngela','passwordLove']
userBalance = [1000,2000,3000]
from datetime import date
today = date.today()
print("Today's date:", today)

if(name in allowedUsers):
    password = input("Your password? \n")
    userId = allowedUsers.index(name)
    
    if(password == allowPassword[userId]):
        print('Welcome %s' % name)
        print('These are the available options:')
        print('1.Withdrawl')
        print('2.Cash Deposit')
        print('3.Complaint')
        currentBalance = userBalance[userId]
        
        selectedOption = int(input('Please select an option' ))
        
        
        if(selectedOption == 1):
            print('you selected %s' % selectedOption)
            howMuch = float(input("How much would you like to withdraw"))
            if(howMuch < currentBalance):
                newBalance = currentBalance - howMuch
            
                print("Take your cash!")
                print("Your balance is %d" % newBalance)
            else:
                print("Insufficient Balance")    
        
        elif(selectedOption == 2):
            print('you selected %s' % selectedOption)
            howMuch = float(input("How much would you like to deposit"))
            newBalance = currentBalance + howMuch
            print("Deposit Successful!")
            print("Your balance is %d" % newBalance)
            
        
        elif(selectedOption == 3):
            print('you selected %s' % selectedOption)
            print('What issue would you like to report?')
            print('Thank you for contacting us!')

        else:
            print('Invalid Option selected, please try again')
    else:
        print('Password Incorrect, please try again')
else:
    print('Name not found, please try again')                     

                

    
                              


