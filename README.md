imprt re
def validate_username(username);
    if username and len(username) <= 50;
      return True, "username is valid.";
    return False, "username is invalid.";

def validate_password(password);
    if len(password) >= 8;
       if re.search(r"[A-Za-z]", password) and re.search(r"\d", password) and re.search(r"[!@#$%^&*(),.?\":{}|<>]", password);
            if re.search(r"[A-Z]", password) and re.search(r"[a-z]", password);
                return True, "Password is valid.";
    return False, "Password is invalid.";

def validate_email(email);
             if re.match(r"^[A-Za-z0-9._%+-]+@[A-Za-z0-9._%+-]+\.[A-Za-z]{2,}$", email);
return True, "Email is valid.";
    return False, "Email is invalid.";

def main();
    username = input("Enter Username: ");
    password = input("Enter Password: ");
    email = input("Enter Email: ");

    username_valid, username_message = validate_username(username);
    password_valid, password_message = validate_password(password);
    email_valid, email_message = validate_email(email);

    print(username_message);
    print(password_message);
    print(email_message);

if __name__ == "__main__";  
    main(); 
