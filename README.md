# Analyst
This is my first Git repository.
Author : Minal Joshi

Bal = 50000
Pin1 = 1010
Pin2 = 2020
print("Welcome to SBI Bank")
name =input("Enter your name : Mr/Mrs/Ms")
att= 3
for x in range (3):
    UPin = int(input("Enter your pin:"))
    if UPin == Pin1:
        print("Your available balnace is ",Bal)
        p= int(input("Enter the amouunt to be withdrawn :"))
        for x in range (3):
            UPin2= int(input("Enter your tranction pin :"))
            if UPin2 == Pin2:
                print("Transction is successful.")
                avlbal= 50000-p
                print("Your available balance is Rs.",avlbal)
                break
        
            else:
                print("Incorrect transction pin,Please try again")
                z = att - x
                print("attempts remaining",z)
                if z==0:
                    print("Your card is blocked.")
                    break
            break
    else:
            print("Incorrect Login")
            z=att-x
            print("Attempts remaining",z)
            if z==0:
                print("Your card is Blocked.")
                break
                    
