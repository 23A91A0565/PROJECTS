import java.util.Scanner;

public class ConsoleCalculatorLoop {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double num1, num2, result;
        char operator;

        System.out.println("=== Simple Calculator ===");
        System.out.println("Type 'exit' at any time to quit.\n");

        while (true) {
            System.out.print("Enter first number: ");
            if (sc.hasNext("exit")) break;
            if (!sc.hasNextDouble()) {
                System.out.println("Invalid input. Please enter a number.");
                sc.next(); continue;
            }
            num1 = sc.nextDouble();

            System.out.print("Enter operator (+, -, *, /): ");
            if (sc.hasNext("exit")) break;
            operator = sc.next().charAt(0);

            System.out.print("Enter second number: ");
            if (sc.hasNext("exit")) break;
            if (!sc.hasNextDouble()) {
                System.out.println("Invalid input. Please enter a number.");
                sc.next(); continue;
            }
            num2 = sc.nextDouble();

            switch (operator) {
                case '+':
                    result = num1 + num2;
                    System.out.println("Result = " + result);
                    break;
                case '-':
                    result = num1 - num2;
                    System.out.println("Result = " + result);
                    break;
                case '*':
                    result = num1 * num2;
                    System.out.println("Result = " + result);
                    break;
                case '/':
                    if (num2 == 0) System.out.println("Error: Division by zero");
                    else System.out.println("Result = " + (num1 / num2));
                    break;
                default:
                    System.out.println("Invalid operator!");
            }

            System.out.println(); // spacing
        }

        System.out.println("Calculator exited.");
        sc.close();
    }
}
