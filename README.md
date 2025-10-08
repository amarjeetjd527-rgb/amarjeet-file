# amarjeet-file
password generator  use in python  a password manager is a secure application that help store manage and generate strong password for all your online account in one place. it keep your password safe using encryption and requires you to remember only one master password
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

# Example usage
print("Generated password:", generate_password(12))