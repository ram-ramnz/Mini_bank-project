# Mini_bank-project
Learning python 
balance = 5000
choice = 0

while choice != 4:
    print("===== ATM =====")
    print("1. Check Balance")
    print("2. Deposit")
    print("3. Withdraw")
    print("4. Exit")
    choice = int(input(""))
    if choice == 1:
        print(f"Your balance is {balance}P")
    elif choice == 2:
        deposit = int(input("Enter Amount: "))
        balance += deposit 
        print(f"Your balance is {balance}P")
    elif choice == 3:
        withdraw = int(input("Enter Amount: "))
        if withdraw > balance:
            print("Insufficient funds.")
        elif withdraw <= balance:
            balance -= withdraw
            print(f"Your balance is {balance}P")
    elif choice == 4:
        print("Thankyou for using the ATM!")
        break
    else:
        print("Invalid Choice.")
