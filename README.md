# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not


def print_initial(name):
    # Define the patterns for each letter
    patterns = {
        'A': ['  *  ', ' * * ', '*****', '*   *', '*   *'],
        ' ': ['     ', '     ', '     ', '     ', '     ']
    }

    name = name.upper()
    if name[0] in patterns:
        for line in patterns[name[0]]:
            print(line)

# Example usage:
name = "Akshit"
print_initial(name)
def print_name_with_for_loop(name):
    for char in name:
        print(char)
print("\nb) Printing the name using a for loop:")
print_name_with_for_loop(name)
def is_palindrome(name):
    # Remove spaces and convert to lowercase for case-insensitive comparison
    name = name.replace(" ", "").lower()
    # Check if the string equals its reverse
    return name == name[::-1]

if is_palindrome(name):
    print("\nc) The name is a palindrome!")
else:
    print("\nc) The name is not a palindrome.")
