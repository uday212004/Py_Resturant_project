# Py_Resturant_project
This is Resturant Project

#Define the menu of restaurant
menu={
    'Tea':25,
    'Coffee':35,
    'Pizza':40,
    'Burger':50,
    'Idli':60,
    'Salad':70,
}

#Greet
print("Welcome to SS Restaurant")
print("Tea: Rs25\nCoffee: Rs35\nPizza: Rs40\nBurger: Rs50\nIdli: Rs60\nSalad: Rs70")

order_total=0
#60 + 50 = 110

item_1 = input("What you want to Order")
if item_1 in menu:
    order_total += menu[item_1] #0 + 50
    print(f"Your item {item_1} has been added to your order")

else:
    print(f"Ordered item {item_1} is out of oredr")

another_order = input("Do you want to order somthing else? (yes/No)")
if another_order=="yes":
    item_2 = input("Enter the name of second item =")
    if item_2 in menu:
        order_total += menu[item_2]
        print(f"Item {item_2} has been added to your order")
    else:
        print(f"ordered item {item_2} in out of order")

another_order = input("Do you want to order somthing else? (yes/No)")
if another_order=="yes":
    item_3= input("Enter what you want to order?")

    if item_3 in menu:
        order_total += menu[item_3]
        print(f"Item {item_3} has been added to your order")
    else:
        print(f"ordered item {item_3} in out of order")

print(f"The total amount of your order to pay is {order_total}")
