# Mycalc
#This is a calculator app for 7-9 year olds.# 

# Functions for calculations
def plus(a, b):      
   return a + b   

def minus(a, b):      
   return a - b   

def times(a, b):      
   return a * b   

def divide(a, b):       
   return a / b       

# Loop until the user decides to stop
while True:
    # Display options to the user
    print("Select a function using the letters shown.")
    print("a. Plus")
    print("b. minus")
    print("c. times")
    print("d. divide")
    
    # User input for choice and numbers
    choice = input("Please enter choice (a/b/c/d): ")        
    num_1 = int(input("Number one: "))    
    num_2 = int(input("Number two: ")) 
          
    # Perform calculation based on choice
    if choice == 'a':    
       print(num_1, " + ", num_2, " = ", plus(num_1, num_2))    
    elif choice == 'b':    
       print(num_1, " - ", num_2, " = ", minus(num_1, num_2))    
    elif choice == 'c':    
       print(num_1, " * ", num_2, " = ", times(num_1, num_2))   
    elif choice == 'd':    
       print(num_1, " / ", num_2, " = ", divide(num_1, num_2))    
    else:    
       print("Incorrect input")   
       
    # Ask user if they want to continue
    continue_choice = input("Would you like to make another calculation? (yes/no): ")
    
    # Check user choice to continue or break
    if continue_choice.lower() == 'no':
        break
    elif continue_choice.lower() != 'yes':
        print("Invalid choice, assuming 'no'.")
        break
