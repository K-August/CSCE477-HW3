# Description
This is a very simple HTML/Javascript file that contains an input for an email and password. 

# Validation
This login form validates three things:
1. There exists an email and password
2. The email has the @ symbol in it
3. The password is at least 8 characters

# Vulnerability
The login page intentially has an XSS vulnerability. When a login fails (after the omitted login handling logic), the page uses innerHTML to put an error message, but it is configured in a way that will execute code.
