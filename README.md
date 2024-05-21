# Brute-Force-Attacker
import string
import random
password = input("Enter your password: ")

char = list(string.printable)

while True:
    var=random.choices(char, k=len(password))
    print(">>>>>>>>",var,"<<<<<<<<")
    ps="".join(var)
    if password==ps:
        print("Your password is : ",ps)
        break
