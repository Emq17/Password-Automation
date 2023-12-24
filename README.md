<h1 align="center">Password Automation</h1>

- The task that I am trying to solve is to automate creating random passwords faster. All the user has to do is input the desired password length they need & the program will spit out random characters with a mixture of uppercase, lowercase letters, numbers & punctuation marks. This will have an output of a strong, diverse password. 
Scams & frauds are on the rise. Online security is becoming a must in today’s generation. Some people lack creativity or are just lazy in choosing passwords that doesn’t relate to their names, birthdays, pet names, etc. This program quickly solves this & by automating it, can help save people time and effort while ensuring that it meets the complexity requirements of certain websites.


<h2>Pseudocode:</h2>


Import necessary modules for string manipulation and random value generation

Define & set variables as lowercase & uppercase letters, digits, & punctuation marks. 

Prompt user for password length 

Check if the user input is correct; If not, display an error and ask for the valid input

Create an empty list (named “pin”) to store the characters for the password

Add variables created above to the list (pin)

Generate a random password by selecting characters from the list based on the specified length user wants

Display the password as the output

(This simplified pseudocode maintains the key steps and logic of the program while removing some of the finer details, maintaining the English language, & creating an overall blueprint to how the program will be designed. This should provide a quick overview of the functionality in a simple yet concise enough form.)

<h2></h2>
While testing the program, I have found that the limit to the possible characters that could be generated only goes up to 94 characters. While this error could be fixed by adding more variations or creativity to generating types of passwords, most websites do not need an influx of this amount of characters for creating passwords. So I left it be. 

![Picture1](https://github.com/Emq17/Password-Automation/assets/147126755/2bbd0d9d-2283-4aa5-9a24-c6b5d5d3ba03)

After playing around with this simple program, everything seems to run smoothly as long as you stay underneath the character count of 95.
This error simply makes sense due to limited characters. Not because of the program itself. 

If the user inputs a letter instead of a number another error will occur unfortunately. The program expects an integer value not a string. It cannot convert a letter into an integer. 
To handle this error created from the user, it is possible to implement error handling and validation in the code (using a try-except block to catch any errors) which could display an error message to the user, prompting them to enter a valid integer instead for the password length. This should provide correct guidance to help ensure the program to run as intended. After realizing the possibility of this happening I went ahead & inputted this code block below:
 “valid_input = False
 
while not valid_input:
    try:
        password_length = int(input("Enter password length: "))
        valid_input = True
    except ValueError:
        print("Invalid input! Please enter a valid integer for the password length.")”

![Picture1](https://github.com/Emq17/Password-Automation/assets/147126755/2a806e0a-bfd7-42d3-928d-76ec8fdce810)

As you can see with above’s screenshot, I have inputted the letter “A” instead of an integer value & it successfully prompted the user instructions on what to do to generate the desired password length. 
