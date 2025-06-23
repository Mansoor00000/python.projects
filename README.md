# python.projects

# PYTHON.py

###The ATM program_______________________________________________________________________________________________
print("welcome to ATM machine")
print('''choose and operation:
       1-withdraw
       2-deposit
       3-check_balance
       4-change_pin''')

op = int(input("enter the operation:"))

bal = 1500
pin = 8585
deposit_limit  >= 5000

if op == 1:
    check_pin = int(input("enter the pin:"))
    if pin == check_pin:
        amt = int(input("enter the amount:"))
        if amt > bal :
         print("insufficient funds")
        elif amt < 0:
         print("only positive number")
        else:
          bal = amt+ bal
          print(f"your money is debited {amt} and  current balance is {bal}")
    else:
           print("wrong pin")
elif op == 2:
    check_pin = int(input("enter the pin:"))
    if pin == check_pin:
        dep_amt = int(input("enter the amount you wish to deposit:"))
        if amt > deposit_limit:
            print("limit exceeded")
        elif amt < 0:
            print("only positive number")
        else:
            new_bal = dep_amt + bal
            print(f"your money is credited {dep_amt} and current bal is {new_bal}")
    else:
        print("wrong pin")
elif op == 3:
    check_pin = int(input("enter the pin:"))
    if pin == check_pin:
        print(f"your balance is : {new_bal}")
    else:
        print("wrong pin")
elif op == 4:
    check_pin = int(input("enter the pin:"))
    if pin == check_pin:
        change_pin = int(input("enter the new pin:"))
        print(f"your new pin is {change_pin}")
    else:
        print("wrong pin")


### The Good burger program_______________________________________________________________________________________________________________________

print("Welcome to Good Burger, Home of the Good Burger")
print('''Please place an order:
        1 - Burger_with_meat_patty 
        2 - Burger_with_chicken_patty 
        3 - Veg_Burger 
        4 - Prawns_Burger''')


Burger_with_meat_patty = 150
Burger_with_chicken_patty = 100
Veg_Burger = 80
Prawns_Burger = 170


order_1 = int(input("Select an option: "))

if order_1 in [1, 2, 3, 4]:
    print('''Would you like to have some extras?
            5 - Mayonnaise 
            6 - Tandoori_sauce 
            7 - Ketchup 
            8 - Veggies ''')

    order_2 = int(input("Select an extra (or 0 to skip): "))

    
    Mayonnaise = 20
    Tandoori_sauce = 30
    Ketchup = 10
    Veggies = 15

    
    if order_1 == 1:
        base_price = Burger_with_meat_patty
    elif order_1 == 2:
        base_price = Burger_with_chicken_patty
    elif order_1 == 3:
        base_price = Veg_Burger
    elif order_1 == 4:
        base_price = Prawns_Burger

    
    if order_2 == 5:
        extra_price = Mayonnaise
    elif order_2 == 6:
        extra_price = Tandoori_sauce
    elif order_2 == 7:
        extra_price = Ketchup
    elif order_2 == 8:
        extra_price = Veggies
    else:
        extra_price = 0  

    
    answer = int(input('''How would you like to eat?
                    1 - Eat In
                    2 - Take Away\n'''))

    total = base_price + extra_price

    if answer == 1:
        print(f"Your total is {total}. Thank you!")
    elif answer == 2:
        print(f"Your total is {total}. Thank you, visit again!")
    else:
        print("Invalid choice")

