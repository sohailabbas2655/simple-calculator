//# simple-calculator
//java project given by sir gulsher
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter first number: ");
        double num1 = scanner.nextDouble();
        
        System.out.print("Enter second number: ");
        double num2 = scanner.nextDouble();

        System.out.print("Enter an operator (+, -, *, /): ");
        char operator = scanner.next().charAt(0);

        double result = 0.0;

        switch (operator) {
            case '+':
                result = num1 + num2;
                break;
            case '-':
                result = num1 - num2;
                break;
            case '*':
                result = num1 * num2;
                break;
            case '/':
                if (num2 != 0) {
                    result = num1 / num2;
                } else {
                    System.out.println("Error! Division by zero is not allowed.");
                }
                break;
            default:
                System.out.println("Invalid operator.");
                break;
        }

        System.out.println("Result: " + result);
        
        scanner.close();
    }
}

//credits 

//leader sohail abbas (csm/2k23/131)
// laid groundwork for the diea

//rizwan hyder (csm/2k23/112)
//provided the idea for the project

//saifullah (csm/2k23/117)
//provided the rest of code for the project

//shahid ali (csm/2k23/129)
//tested and debugged the code and uploaded on github
