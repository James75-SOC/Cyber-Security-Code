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

# using the append function to add users and computers to an approved list
# Assign `approved_users` to a list of approved usernames
approved_users = ["elarson", "bmoreno", "tshah", "sgilmore", "eraab"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "2ye3lzg", "4n482ts", "a307vir"]
# Assign `new_user` to the username of a new approved user
new_user = "gesparza"
# Assign `new_device` to the device ID of the new approved user
new_device = "3rcv4w6"
# Add that user's username and device ID to `approved_users` and `approved_devices` respectively
approved_users.append("gesparza")
approved_devices.append("3rcv4w6")
# Display the contents of `approved_users`
print(approved_users)
# Diplay the contents of `approved_devices`
print(approved_devices)
# use the remove() function to take names off the lists

# this code searches a list of users to check if they are on a list using a conditional statement
approved_users = ["elarson", "bmoreno", "sgilmore", "eraab", "gesparza"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "4n482ts", "a307vir", "3rcv4w6"]
# Assign `username` to a username
username = "sgilmore"
# Conditional statement
if username in approved_users:
    print("The user", username, "is approved to access the system.")
else:
    print("the user", username, "is not approved to access the system.")

# This code returns the position of a givien value in a list
# Assign `approved_users` to a list of approved usernames
approved_users = ["elarson", "bmoreno", "sgilmore", "eraab", "gesparza"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "4n482ts", "a307vir", "3rcv4w6"]
# Assign `username` to a username
username = "sgilmore"
# Assign `ind` to the index of `username` in `approved_users`
ind = approved_users.index(username)
# Display the value of `ind`
print(ind)

# this code demonstrates how you can find an index in one list and then use this index to display connected information in another list
# Assign `approved_users` to a list of approved usernames
approved_users = ["elarson", "bmoreno", "sgilmore", "eraab", "gesparza"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "4n482ts", "a307vir", "3rcv4w6"]
# Assign `username` to a username
username = "sgilmore"
# Assign `ind` to the index of `username` in `approved_users`
ind = approved_users.index(username)
# Display the device ID at the index that matches the value of `ind` in `approved_devices`
print(approved_devices[ind])

# this code determines if a username and device ID correspond. The conditional checks if the username is an element of the approved_devices and if the device_id stored at the same index as username matches the device_id entered.
# Assign `approved_users` to a list of approved usernames
approved_users = ["elarson", "bmoreno", "sgilmore", "eraab", "gesparza"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "4n482ts", "a307vir", "3rcv4w6"]
# Assign `username` to a username
username = "sgilmore"
# Assign `device_id` to a device ID
device_id = "4n482ts"
# Assign `ind` to the index of `username` in `approved_users
ind = approved_users.index(username)
# Conditional statement
if username in approved_users and device_id == approved_devices[ind]:
    print("The username", username, "is approved to access the system.")
    print(device_id, "is the assigned device for", username)

# this matches the above code but runs an elif statement incase things don't match i.e like in this example
# Assign `approved_users` to a list of approved usernames
approved_users = ["elarson", "bmoreno", "sgilmore", "eraab", "gesparza"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "4n482ts", "a307vir", "3rcv4w6"]
# Assign `username` to a username
username = "sgilmore"
# Assign `device_id` to a device ID
device_id = "8rp2K75"
# Assign `ind` to the index of `username` in `approved_users`
ind = approved_users.index(username)
if username in approved_users and device_id == approved_devices[ind]:
    print("The user", username, "is approved to access the system.")
    print(device_id, "is the assigned device for", username)
elif username in approved_users and device_id != approved_devices[ind]:
# Handles the case when `username` belongs to `approved_users` but element at `ind` in `approved_devices` does not match `device_id`,
# and displays two messages accordingly
    print("The user", username, "is approved to access the system, but", device_id, "is not their assigned device.")


#  A complete algorithm using a function and conditionals to automate the login process. In the following code, a nested conditional is used to achieve the goals of the algorithm. There is a conditional statement inside of another conditional statement. The outer conditional handles the case when the username is approved and the case when username is not approved. The inner conditional, which is placed inside the first if statement, handles the case when the username is approved and the device_id is correct, as well as the case when the username is approved and the device_id is incorrect.
# Assign `approved_users` to a list of approved usernames
approved_users = ["elarson", "bmoreno", "sgilmore", "eraab", "gesparza"]
# Assign `approved_devices` to a list of device IDs that correspond to the usernames in `approved_users`
approved_devices = ["8rp2k75", "hl0s5o1", "4n482ts", "a307vir", "3rcv4w6"]
# Define a function named `login` that takes in two parameters, `username` and `device_id`
def login(username, device_id):

    if username in approved_users:
       print("The user", username, "is approved to access the system.")
       # assign `ind` to the index of `username` in `approved_users`,
        ind = approved_users.index(username)
        # and execute the following conditional
        # If `device_id` matches the element at the index `ind` in `approved_devices`,
        if device_id == approved_devices[ind]:
        # then display "______ is the assigned device for ______"
        print(device_id, "is the assigned device for", username)
        
    else:
        print(device_id, "is not their assigned device.")
    else:
        print("The username", username, "is not approved to access the system.")
# Call the function defined to experiment with different username and device_id combinations
login("elarson", "3rcv4w6")


#notes
# 1) Indexing a list is similar to indexing a string. Index values start at 0.
# 2) The .append() method helps you add new elements to the end of lists.
# 3) The .remove() method helps you remove elements from lists.
# 4) The .index() method can be used on different types of sequences. They can be used not only with strings, but also with lists.
# 5) With a list, the .index() method allows you to identify the position where a specified element is located in that list.
# 6) If two lists contain information that correspond to each other in a specific order, you can use indices to pair elements from the lists together.
# 7) Functions can be used to develop algorithms. When defining a function, you must specify the parameters it takes in and the actions it should execute.

import re #this command imports the regular expression module
# Assign `devices` to a string containing device IDs, each device ID represented by alphanumeric characters
devices = "r262c36 67bv8fy 41j1u2e r151dm4 1270t3o 42dr56i r15xk9h 2j33krk 253be78 ac742a1 r15u9q5 zh86b2l ii286fq 9x482kt 6oa6m6u x3463ac i4l56nq g07h55q 081qc9t r159r1u"
# Assign `target_pattern` to a regular expression pattern for finding device IDs that start with "r15"
target_pattern = "r15\w+"
# Use `re.findall()` to find the device IDs that start with "r15" and display the results
print(re.findall(target_pattern, devices))


# Assign `log_file` to a string containing username, date, login time, and IP address for a series of login attempts 
log_file = "eraab 2022-05-10 6:03:41 192.168.152.148 \niuduike 2022-05-09 6:46:40 192.168.22.115 \nsmartell 2022-05-09 19:30:32 192.168.190.178 \narutley 2022-05-12 17:00:59 1923.1689.3.24 \nrjensen 2022-05-11 0:59:26 192.168.213.128 \naestrada 2022-05-09 19:28:12 1924.1680.27.57 \nasundara 2022-05-11 18:38:07 192.168.96.200 \ndkot 2022-05-12 10:52:00 1921.168.1283.75 \nabernard 2022-05-12 23:38:46 19245.168.2345.49 \ncjackson 2022-05-12 19:36:42 192.168.247.153 \njclark 2022-05-10 10:48:02 192.168.174.117 \nalevitsk 2022-05-08 12:09:10 192.16874.1390.176 \njrafael 2022-05-10 22:40:01 192.168.148.115 \nyappiah 2022-05-12 10:37:22 192.168.103.10654 \ndaquino 2022-05-08 7:02:35 192.168.168.144"
# Assign `pattern` to a regular expression pattern that will match with IP addresses of the form xxx.xxx.xxx.xxx
pattern = "\d\d\d\.\d\d\d\.\d\d\d\.\d\d\d" # this regular expression matches with a section of 3 digits followed by a period
print(re.findall(pattern, log_file))


# Assign `log_file` to a string containing username, date, login time, and IP address for a series of login attempts 
log_file = "eraab 2022-05-10 6:03:41 192.168.152.148 \niuduike 2022-05-09 6:46:40 192.168.22.115 \nsmartell 2022-05-09 19:30:32 192.168.190.178 \narutley 2022-05-12 17:00:59 1923.1689.3.24 \nrjensen 2022-05-11 0:59:26 192.168.213.128 \naestrada 2022-05-09 19:28:12 1924.1680.27.57 \nasundara 2022-05-11 18:38:07 192.168.96.200 \ndkot 2022-05-12 10:52:00 1921.168.1283.75 \nabernard 2022-05-12 23:38:46 19245.168.2345.49 \ncjackson 2022-05-12 19:36:42 192.168.247.153 \njclark 2022-05-10 10:48:02 192.168.174.117 \nalevitsk 2022-05-08 12:09:10 192.16874.1390.176 \njrafael 2022-05-10 22:40:01 192.168.148.115 \nyappiah 2022-05-12 10:37:22 192.168.103.10654 \ndaquino 2022-05-08 7:02:35 192.168.168.144"
# Update `pattern` to a regular expression pattern that will match with IP addresses with any variation in the number of digits per segment
pattern = "\d+\.\d+\.\d+\.\d+" # Placing + after \d results in \d+, which will match with one or more digits.
# Use the `re.findall()` function on `pattern` and `log_file` to extract the IP addresses of the updated form specifed above and display the results
print(re.findall(pattern, log_file))


# Assign `log_file` to a string containing username, date, login time, and IP address for a series of login attempts 
log_file = "eraab 2022-05-10 6:03:41 192.168.152.148 \niuduike 2022-05-09 6:46:40 192.168.22.115 \nsmartell 2022-05-09 19:30:32 192.168.190.178 \narutley 2022-05-12 17:00:59 1923.1689.3.24 \nrjensen 2022-05-11 0:59:26 192.168.213.128 \naestrada 2022-05-09 19:28:12 1924.1680.27.57 \nasundara 2022-05-11 18:38:07 192.168.96.200 \ndkot 2022-05-12 10:52:00 1921.168.1283.75 \nabernard 2022-05-12 23:38:46 19245.168.2345.49 \ncjackson 2022-05-12 19:36:42 192.168.247.153 \njclark 2022-05-10 10:48:02 192.168.174.117 \nalevitsk 2022-05-08 12:09:10 192.16874.1390.176 \njrafael 2022-05-10 22:40:01 192.168.148.115 \nyappiah 2022-05-12 10:37:22 192.168.103.10654 \ndaquino 2022-05-08 7:02:35 192.168.168.144"
# Assign `pattern` to a regular expression that matches with all valid IP addresses and only those 
pattern = "\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}" # using curly brackets in a expression limits search to 3 places per section
# Use `re.findall()` on `pattern` and `log_file` and assign `valid_ip_addresses` to the output 
valid_ip_addresses = re.findall(pattern, log_file)
# Display the contents of `valid_ip_addresses`
print(valid_ip_addresses)

# this code searches through a log file and returns flagged IP addresses for further analsis
# Assign `log_file` to a string containing username, date, login time, and IP address for a series of login attempts 
log_file = "eraab 2022-05-10 6:03:41 192.168.152.148 \niuduike 2022-05-09 6:46:40 192.168.22.115 \nsmartell 2022-05-09 19:30:32 192.168.190.178 \narutley 2022-05-12 17:00:59 1923.1689.3.24 \nrjensen 2022-05-11 0:59:26 192.168.213.128 \naestrada 2022-05-09 19:28:12 1924.1680.27.57 \nasundara 2022-05-11 18:38:07 192.168.96.200 \ndkot 2022-05-12 10:52:00 1921.168.1283.75 \nabernard 2022-05-12 23:38:46 19245.168.2345.49 \ncjackson 2022-05-12 19:36:42 192.168.247.153 \njclark 2022-05-10 10:48:02 192.168.174.117 \nalevitsk 2022-05-08 12:09:10 192.16874.1390.176 \njrafael 2022-05-10 22:40:01 192.168.148.115 \nyappiah 2022-05-12 10:37:22 192.168.103.10654 \ndaquino 2022-05-08 7:02:35 192.168.168.144"
# Assign `pattern` to a regular expression that matches with all valid IP addresses and only those 
pattern = "\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
# Use `re.findall()` on `pattern` and `log_file` and assign `valid_ip_addresses` to the output 
valid_ip_addresses = re.findall(pattern, log_file)
# Assign `flagged_addresses` to a list of IP addresses that have been previously flagged for unusual activity
flagged_addresses = ["192.168.190.178", "192.168.96.200", "192.168.174.117", "192.168.168.144"]
# Iterative statement begins here
# Loop through `valid_ip_addresses` with `address` as the loop variable
for address in valid_ip_addresses:
    # Conditional begins here
    # If `address` belongs to `flagged_addresses`, display "The IP address ______ has been flagged for further analysis."
    if address in flagged_addresses:
        print("The IP address", address, "has been flagged for further analysis.")
    # Otherwise, display "The IP address ______ does not require further analysis."
    else:
        print("this IP address", address, "does not require further analysis")


# open, read and append to files in Python, this example uses .txt file
# Assign `import_file` to the name of the text file that you want to create
import_file = "allow_list.txt"
# Assign `ip_addresses` to a list of IP addresses that are allowed to access the restricted information
ip_addresses = "192.168.218.160 192.168.97.225 192.168.145.158 192.168.108.13 192.168.60.153 192.168.96.200 192.168.247.153 192.168.3.252 192.168.116.187 192.168.15.110 192.168.39.246"
# Create a `with` statement to write to the text file 
with open(import_file, "w") as file:
    # Write `ip_addresses` to the text file
    file.write(ip_addresses)
# Create a `with` statement to read in the text file 
with open(import_file, "r") as file:
    # Read the file and store the result in a variable named `text`
    text = file.read()
# Display the contents of `text`
print(text)

# removing IP adresses from an allow list using a function
# Define a function named `update_file` that takes in two parameters: `import_file` and `remove_list`
def update_file(import_file, remove_list):
  # Build `with` statement to read in the initial contents of the file
  with open(import_file, "r") as file:
    # Use `.read()` to read the imported file and store it in a variable named `ip_addresses`
    ip_addresses = file.read()
  # Use `.split()` to convert `ip_addresses` from a string to a list
  ip_addresses = ip_addresses.split()
  # Build iterative statement
  # Name loop variable `element`
  # Loop through `ip_addresses`
  for element in ip_addresses:
    # Build conditional statement
    # If current element is in `remove_list`,
    if element in remove_list:
      # then current element should be removed from `ip_addresses`
      ip_addresses.remove(element)
  # Convert `ip_addresses` back to a string so that it can be written into the text file     
  ip_addresses = " ".join(ip_addresses)
  # Build `with` statement to rewrite the original file
  with open(import_file, "w") as file:
    # Rewrite the file, replacing its contents with `ip_addresses`
    file.write(ip_addresses)
# Call `update_file()` and pass in "allow_list.txt" and a list of IP addresses to be removed
update_file("allow_list.txt", ["192.168.25.60", "192.168.140.81", "192.168.203.198"])
# Build `with` statement to read in the updated file
with open("allow_list.txt", "r") as file:
  # Read in the updated file and store the contents in `text`
  text = file.read()
# Display the contents of `text`
print(text)
