Password Generator Project
Overview
This project is a secure and customizable password generator in Python, which utilizes Python's built-in secrets module to generate strong, random passwords which meet user-defined constraints for length (e.g., number of characters) and types of characters.
Features
Generate passwords of customizable length (default is 16 characters)
Ensure inclusion of:
Numbers (digits)
Special characters (symbols)
Uppercase letters
Lowercase letters
Generate passwords using a secure random generator, so passwords are cryptographically strong
Validate generated password using constraints before outputting
How It Works
The generate_password function:
Puts letters, digits, and symbols into a pool of possible characters
Uses secure random selection to generate a random password of a specified length
Uses regular expressions (i.e., the re module) to ensure that the password contains at least the minimum number of required numbers, special characters, uppercase letters, and lowercase letters
Repeats generation until all constraints are satisfied
Usage
Execute the script:
python3 Password_Generator_Project.py
Sample output:
Generated password: A7!kd9#LmQ2@Tp3Z
Customization
Customize the function parameters:
generate_password(length=20, nums=2, special_chars=3, uppercase=2, lowercase=4)
to customize the password length and minimum counts of required characters.
Requirements
Python 3.x
No external libraries (i.e., uses built-in modules secrets, string, and re)
License
This project is open-source and
