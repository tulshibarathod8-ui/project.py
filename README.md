# project.py

print("Welcome to the Pattern Generator and Number Analyzer!")

while True:
    print("\nSelect an option: ")
    print("1. Generate a Pattern")
    print("2. Analyze a Range of Numbers")
    print("3. Exit")

    choice = int(input("Enter your choice: "))


    match choice:
        case 1:
            rows = int(input("Enter the number of rows for the pattern: "))
            if(rows > 0):
                print("\nPattern:")

                for i in range(1,rows+1):
                   for j in range(1,i+1):
                       print("*",end="")
                   print()
            else:    
                print("Error: Number of rows must be positive integer.")   

        case 2:
            start = int(input("\nEnter the start of range: "))
            end = int(input("Enter the end of range: "))
            if(start > end):
                print("Error: The end of the range must be greater than the start.")
            else:
                total_sum = 0
                for num in range(start,end+1):
                   if(num % 2 == 0 ):
                       print("Number",num,"is Even")
                   else:
                       print("Number",num,"is Odd")
                       
                   total_sum += num
                print(f"Sum of all numbers from {start} to {end} is: {total_sum}") 

        case 3:
            print("Exiting the program. Goodbye!")
            break

        case _:
            print("Error: Invalid choice! Please enter valid choice.")
