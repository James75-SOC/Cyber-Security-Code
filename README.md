# here's a simple conditional statement in Python that checks whether the user's system is up-to-date:
user_system = "OS 2"  # You can replace this with the actual OS of the user
if user_system == "OS 2":
    print("Your system is up-to-date.")
else:
    print("Your system is not up-to-date.")
# In this example, the code checks if the user_system variable is equal to "OS 2" and then prints a corresponding message based on the result. 
# If the user's system is OS 2, it will print "Your system is up-to-date." Otherwise, it will print "Your system is not up-to-date."


# Here's the modified code with different values assigned to the user_system variable:
user_system = "OS 1"  # You can replace this with "OS 2" or "OS 3" to test different cases
if user_system == "OS 2":
    print("Your system is up-to-date.")
else:
    print("Your system is not up-to-date.")
# You can change the value of user_system to "OS 2" or "OS 3" to see how the conditional statement responds to different operating systems.


# Here's the modified code to include all three operating systems:
user_system = "OS 1"  # Replace with "OS 2" or "OS 3" to test different cases
if user_system == "OS 2":
    print("Your system is up-to-date.")
elif user_system == "OS 1" or user_system == "OS 3":
    print("Your system is not up-to-date.")
else:
    print("Invalid operating system.")
# In this version, the if statement checks if the user_system is "OS 2" and prints the corresponding message. If it's "OS 1" or "OS 3," it prints a message indicating that the system is not up-to-date. If the user_system doesn't match any of these options, it prints an "Invalid operating system" message.



# Here's a refined version of your code using logical operators:
user_system = "OS 1"  # Replace with "OS 2" or "OS 3" to test different cases
if user_system == "OS 2":
    print("No update needed.")
elif user_system == "OS 1" or user_system == "OS 3":
    print("Update needed.")
else:
    print("Invalid operating system.")
# This version uses logical operators (or) to combine the conditions for "OS 1" and "OS 3" in a single elif statement, making the code more concise and readable.



# Here's a simple Python code snippet that checks if the username is among the approved users and displays a corresponding message:
approved_user1 = "elarson"
approved_user2 = "bmoreno"
username = "bmoreno"
if username == approved_user1 or username == approved_user2:
    print("You are approved to access this device.")
else:
    print("You do not have access to this device.")
# In this example, it checks if the username is equal to either approved_user1 or approved_user2. If it is, it prints a message saying the user is approved; otherwise, it prints a message stating that the user does not have access to the device.




# Here's a conditional statement in Python that checks the value of organization_hours and displays the appropriate message:
organization_hours = True  # Replace with False to test different cases
if organization_hours:
    print("Login attempt made during organization hours.")
else:
    print("Login attempt made outside of organization hours.")
# This code uses the if statement to check if organization_hours is True. If it is, it prints the message for a login attempt made during organization hours. If organization_hours is False, it prints the message for a login attempt made outside of organization hours.



approved_list = ["elarson", "bmoreno", "tshah", "sgilmore", "eraab"]
username = "bmoreno"
organization_hours = True
if username in approved_list and organization_hours:
    print("Login attempt made by an approved user during organization hours.")
else:
    print("Username not approved or login attempt made outside of organization hours.")
# This way, the if statement checks if both conditions (username in approved_list and organization_hours) are true before printing the appropriate message. It makes the code more compact and readable.




