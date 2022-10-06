# Learning
Code and improved code

Print numbers from 1 to n as a string with no spaces
# My code
if __name__ == '__main__':
    n = int(input())
    output=""
    for numbers in range(1, n+1):
        output+= str(numbers)
    print(output)

Improved code
if __name__ == '__main__':
    n = int(input())
    if 1 <= n <= 150:
        for i in range(n):
            print(i+1, end='')
            
           
# Mutating Strings 
# Two Methods
# A. 

def mutate_string(string, position, character):
    return(string[:position] + character + string[position + 1:])

# B. 

def mutate_string(string, position, character):
    string_list = list(string)
    string_list[position] = character
    string = "".join(string_list)
    return string
