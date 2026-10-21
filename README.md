# project.py

print("1. Sandwich")
print("2. Pizza")
print("3. Burger")

choice = int(input("Enter your choice (1-3): "))
             
match choice:
    case 1:
        print("\nSandwich Menu")
        print("1. Veg Sandwich")
        print("2. Cheese Sandwich")
        print("3. Grilled Sandwich")

        every_choice = int(input("Enter sandwich choice: "))

        match every_choice:
            case 1:
                print("You ordered Veg Sandwich")
            case 2:
                print("You ordered Cheese Sandwich")
            case 3:
                print("You ordered Grilled Sandwich")
            case _:
                print("Invalid sandwich choice")

    case 2:
        print("\nPizza Menu")
        print("1. Thin Crust Pizza")
        print("2. Cheese Burst Pizza")
        print("3. Fresh Dough Pizza")

        sub_choice = int(input("Enter pizza choice: "))

        match sub_choice:
            case 1:
                print("You ordered Thin Crust Pizza")
            case 2:
                print("You ordered Cheese Burst Pizza")
            case 3:
                print("You ordered Fresh Dough Pizza")
            case _:
                print("Invalid pizza choice")

    case 3:
        print("\nBurger Menu")
        print("1. Veg Burger")
        print("2. Cheese Burger")
        print("3. Double Patty Burger")

        sub_choice = int(input("Enter burger choice: "))

        match sub_choice:
            case 1:
                print("You ordered Veg Burger")
            case 2:
                print("You ordered Cheese Burger")
            case 3:
                print("You ordered Double Patty Burger")
            case _:
                print("Invalid burger choice")

    case _:
        print("Invalid menu choice")
    
