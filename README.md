Problem 1
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


Problem 2
public class DecimalToBinaryConverter {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Prompt the user for input
        System.out.print("Enter a positive decimal number: ");
        int decimal = scanner.nextInt();
        
        // Validate input
        if (decimal < 0) {
            System.out.println("Please enter a positive number.");
        } else {
            // Convert decimal to binary
            String binary = convertDecimalToBinary(decimal);
            System.out.println("Decimal: " + decimal);
            System.out.println("Binary: " + binary);
        }
        
        scanner.close();
    }

    public static String convertDecimalToBinary(int decimal) {
        if (decimal == 0) {
            return "0";
        }
        
        StringBuilder binary = new StringBuilder();
        while (decimal > 0) {
            int remainder = decimal % 2;
            binary.insert(0, remainder);
            decimal = decimal / 2;
        }
        return binary.toString();
    }


    Problem 3
    function rightAngleTriangle(rows, char) {
  for (let i = 1; i <= rows; i++) {
    let str = "";
    for (let j = 1; j <= i; j++) {
      str += char;  // Replace * with your desired character
    }
    console.log(str);
  }
}


Problem 4
public class Main {
    public static void main(String[] args) {
        
        List<Integer> numbers = new ArrayList<>();
        numbers.add(1);
        numbers.add(2);
        numbers.add(3);
        numbers.add(4);
        numbers.add(5);
        numbers.add(6);
        numbers.add(7);
        numbers.add(8);
        numbers.add(9);
        System.out.println("List of integers: " + numbers);
    }
}
