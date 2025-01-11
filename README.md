
import java.util.Scanner;

public class SumOfDigits {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter a number
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();

        // Initialize the sum
        int sum = 0;

        // Calculate the sum of digits
        while (number != 0) {
            sum += number % 10; // Get the last digit and add to sum
            number /= 10;       // Remove the last digit
        }

        // Display the result
        System.out.println("The sum of the digits is: " + sum);

        scanner.close();
    }
}


OUTPUT:

PS C:\Users\MY\OneDrive\Pictures\Documents\java emc 1>  & 'C:\Users\MY\AppData\Roaming\Code\User\workspaceStorage\09ba20b68fc885bcf32d210e84cb47ec\redhat.java\jdt_ws\java emc 1_2ecfe798\bin' 'SumOfDigits'
Enter a number: 6
The sum of the digits is: 6
PS C:\Users\MY\OneDrive\Pictures\Documents\java emc 1>


