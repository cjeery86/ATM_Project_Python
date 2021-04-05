# ATM_Project_Python
ATM_Code
print("Welcome to Pyhton Bank, where money slithers into your Pockets and not out")

#print("---------------------------------------------------------------------------------")
#print("\n   JC&AH 2021 and Beyond-Do what it takes for 360 Success!  ")                                                                              )
#print("\n------------------------------------------------------------------------------")            
name = input("What is your name? \n")
allowedUsers = ['Jerry','Angela','Love']
allowPassword =['passwordJerry','passwordAngela','passwordLove']
welcome = ["Welcome to Pyhton Bank"]
accountBalance = [1,000,000, 2,000,000, 3,000,000]
transaction = ["withdrawl", "deposit","comment"]

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
        if selectedOption == 1:
           #while option !=0
           trans = input["transaction:"]
        #if trans == ('withdrawl')
        selectedOption = int(input('Please select an option'))
        print(selectedOption ==1)
        print("You have selected %s" % seletedOption)
        if(selectedOption == 1):        
            print('you selected %s' % selectedOption)
            print('How much would you like to withdraw?')
            #elif (trans == 1.withdrawl):
            amount = input ("enter amount")
            if amount >0:
                print("collect your cash, thanks stopping in!")
            else:
                print("insufficient funds")
                                                   
                         
                         
            if withdrawl >0:
            #elif trans == 'deposit':
            amount = input ("enter amount")
            if deposit >0:
            elif(selectedOption == 2):
            print('How much would you like to deposit?')
            elif trans == 'deposit':
            deposit input ("enter amount to deposit")
            if deposit >0:
            print("Your deposit it has been successful")
            else:
                print("enter valid amount")
                print('you selected %s' % selectedOption)
            elif(selectedOption == 3):
                print('What issue will you to report?')
                print('Thank you for contacting us!')
                print('Please call 1888-252-2525, ask for Angela')
                print('you selected %s' % selectedOption)
        else:
            print('Invalid Option selected, please try again')
    else:
        print('Password Incorrect, please try again')
else:
    print('Name not found, please try again')
elif option == 0:
    break     
