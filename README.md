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


 
# The condition in the while loop should be checking if connection_attempts is less than 3
connection_attempts = 0
while connection_attempts < 3:
    print("connection could not be established") 
    connection_attempts = connection_attempts + 1
# This way, the loop will run as long as connection_attempts is less than 3, and it will print the specified string three times.


ip_addresses = ["192.168.142.245", "192.168.109.50", "192.168.86.232", "192.168.131.147", "192.168.205.12", "192.168.200.48"]
for ip_address in ip_addresses:
    print(ip_address)
# In each iteration, it will print a single element from the ip_addresses list.


# This code checks if each IP address in ip_addresses is present in the allow_list and prints whether it's allowed or not.
allow_list = ["192.168.243.140", "192.168.205.12", "192.168.151.162", "192.168.178.71", "192.168.86.232", "192.168.3.24", "192.168.170.243", "192.168.119.173"]
ip_addresses = ["192.168.142.245", "192.168.109.50", "192.168.86.232", "192.168.131.147","192.168.205.12", "192.168.200.48"]          
for i in ip_addresses:
    if i in allow_list:
        print("IP address", i, "is allowed")    
    else:
        print("IP address", i, "is not allowed")


allow_list = ["192.168.243.140", "192.168.205.12", "192.168.151.162", "192.168.178.71", "192.168.86.232", "192.168.3.24", "192.168.170.243", "192.168.119.173"]
ip_addresses = ["192.168.142.245", "192.168.109.50", "192.168.86.232", "192.168.131.147", "192.168.205.12", "192.168.200.48"]
for i in ip_addresses:
    if i in allow_list:
        print("IP address", i, "is allowed")
    else:
        print("Further investigation of login activity required")
        break
#  if any IP address is not allowed, it will print the investigation message and then break out of the loop.


employee_ids = set()  # Using a set to store unique employee IDs
current_id = 5000
while current_id <= 5150:
    if current_id % 5 == 0:
        employee_ids.add(current_id)
        print("Generated employee ID:", current_id)
    current_id += 5  # Increment by 5
print("All unique employee IDs for the Sales department have been generated.")
# This script initializes an empty set to store unique employee IDs. It then uses a while loop to iterate through numbers from 5000 to 5150 (inclusive). If the current number is divisible by 5, it adds it to the set of employee IDs and prints the generated ID. The loop continues until it has checked all numbers in the specified range.

# FUNCTIONS
def remaining_login_attempts(maximum_attempts, total_attempts):     # create a function and add parameters
    return maximum_attempts - total_attempts       # use a return statement to return a calculation
remaining_attempts = remaining_login_attempts(3, 3) # add the argument 3, 3 into the function and add the whole thing to a variable
if remaining_attempts <= 0:   # use a conditional statement to return whats in the print function if remaining attempts is less than or equal to 0
    print("Your account is locked")
# In this example, the message prints because the calculation in the function results in 0


# Define a function named `analyze_logins()` that takes in three parameters, `username`, `current_day_logins`, and `average_day_logins`
 def analyze_logins(username, current_day_logins, average_day_logins):
     print("Current day login total for", username, "is", current_day_logins) # Display a message about how many login attempts the user has made that day
     print("Average logins per day for", username, "is", average_day_logins) # Display a message about average number of login attempts the user has made that day
     login_ratio = current_day_logins / average_day_logins # Calculate the ratio of the logins made on the current day to the logins made on an average day, storing in a variable named `login_ratio`
     return login_ratio # Return the ratio
login_analysis = analyze_logins("ejones", 9, 3) # Call `analyze_logins() and store the output in a variable named `login_analysis`
if login_analysis >= 3:
    print("Alert! This account has more login activity than normal.") # Conditional statement that displays an alert about the login activity if it's more than normal





