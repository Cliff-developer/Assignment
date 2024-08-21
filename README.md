# Assignment
# steps required to install Git on a Windows machine
Go to the official Git website and download the latest version for Windows.
After downloading, open the installer to begin the installation process.
Choose where you want Git to be installed on your machine.
Select Components and Pay attention to the Git Bash Git GUI
Choose the option to use Git from the command line and 3rd-party software.
Select "Use OpenSSH,"
Choose "Checkout Windows-style, commit Unix-style line endings"
Select "Use MinTTY"
Complete the Installation

# Explain the purpose of configuring your username and email in Git. How does this configuration affect your Git workflow?
The purpose of these configurations is to associate your identity with your Git commits. The username and email are embedded in each commit, helping to identify who made the changes.
Impact on Workflow is that configuring your username and email ensures that your contributions are correctly attributed, especially in collaborative projects. If not configured, your commits might be attributed to an unknown user, which could cause confusion in team settings.

# What is an SSH key, and why is it recommended to connect Git to GitHub using SSH? Provide a step-by-step guide for generating and adding an SSH key to GitHub.
An SSH key is a pair of cryptographic keys (private and public) used to authenticate a secure connection between your machine and GitHub.
SSH is recommended because it is more secure than using HTTPS and does not require entering your GitHub username and password every time you push or pull changes.
The step-by-Step Guide to Generate and Add an SSH Key:
Generate SSH Key
Add SSH Key to the SSH-Agent
Add SSH Key to GitHub


# Provide the Git commands for the following tasks and explain what each command does:
1. Initialize a new Git repository- git init .This creates a new Git repository in the current directory, allowing you to start tracking changes to files.
2. Clone an existing repository- git clone <repository_url> .This command copies an existing repository (including its history) from GitHub or another remote location to your local machine.
3. Add all modified files to the staging area- git add .This stages all modified and new files in the current directory, preparing them for a commit.
4. Commit the changes with a message -git commit -m "Your commit message" This saves the changes in the staging area to the repository with a descriptive message explaining what was changed.
5. Push the changes to the main branch on GitHub -git push origin main .This uploads your committed changes from the local repository to the remote repository on GitHub, specifically to the main branch.

# After setting up Git and GitHub, how can you verify that your local Git setup is properly connected to GitHub? What is the expected output?
You can verify the connection by using the command ssh -T git@github.com .This command tests the SSH connection to GitHub. The expected output is a success message like “Hi username! You've successfully authenticated, but GitHub does not provide shell access.” This confirms that your local Git setup is properly connected to GitHub.

# Python Navigator Questions
#Explain the concept of variables and data types in Python. Provide an example in Python where different data types (integer, string, and boolean) are used.
Variables are used to store data in a program. They are like containers that hold values which can be changed throughout the program.A example;
age = 25  # Integer
name = "Alice"  # String
is_student = True  # Boolean

print(age, name, is_student)


# What is control flow in Python? Write a Python script using if, elif, and else statements to check if a number is positive, negative, or zero.
Control flow refers to the order in which individual statements, instructions, or function calls are executed or evaluated in a program.An example script;
num = 10

if num > 0:
    print("The number is positive")
elif num < 0:
    print("The number is negative")
else:
    print("The number is zero")

# Differentiate between for loops and while loops in Python. Provide examples of each where a list of numbers is iterated over, and only even numbers are printed.
For Loops are used for iterating over a sequence (like a list, tuple, dictionary, set, or string) and executing a block of code multiple times while While Loops repeatedly execute a block of code as long as a specified condition is True.
For loop example;
numbers = [1, 2, 3, 4, 5, 6]

for num in numbers:
    if num % 2 == 0:
        print(num)
While loop example;
numbers = [1, 2, 3, 4, 5, 6]
index = 0

while index < len(numbers):
    if numbers[index] % 2 == 0:
        print(numbers[index])
    index += 1


# Define what a function is in Python and explain its importance. Write a Python function that takes two arguments (a and b) and returns their sum.
A function is a block of code that only runs when it is called. Functions are important because they allow you to reuse code, making your program more modular and easier to understand.
python function;
def add(a, b):
    return a + b

result = add(3, 5)
print(result)


# Compare lists and dictionaries in Python. How would you use a list and a dictionary to store the names and ages of three people? Provide a Python code example.
Lists are Ordered collections of items which are indexed by position (starting from 0) while Dictionaries are Unordered collections of items which are indexed by keys.
Examples;
# Using a list to store names
names = ["Alice", "Bob", "Charlie"]

# Using a dictionary to store names and corresponding ages
people = {"Alice": 25, "Bob": 30, "Charlie": 35}

print(names)
print(people)



