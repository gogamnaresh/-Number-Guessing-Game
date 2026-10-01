import java.util.Scanner;
import java.util.Random;

public class NumberGuessingGame {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        Random random = new Random();

        System.out.println("================================");
        System.out.println("      NUMBER GUESSING GAME");
        System.out.println("================================");

        System.out.println("\nChoose Difficulty:");
        System.out.println("1. Easy   (1 - 50)");
        System.out.println("2. Medium (1 - 100)");
        System.out.println("3. Hard   (1 - 500)");

        System.out.print("\nEnter your choice: ");
        int choice = scanner.nextInt();

        int maxNumber;

        if (choice == 1) {
            maxNumber = 50;
        } 
        else if (choice == 2) {
            maxNumber = 100;
        } 
        else if (choice == 3) {
            maxNumber = 500;
        } 
        else {
            System.out.println("Invalid choice!");
            scanner.close();
            return;
        }

        int secretNumber = random.nextInt(maxNumber) + 1;
        int guess;
        int attempts = 0;

        System.out.println("\nI selected a number between 1 and " + maxNumber);
        System.out.println("Try to guess it!");

        do {
            System.out.print("\nEnter your guess: ");
            guess = scanner.nextInt();
            attempts++;

            if (guess < secretNumber) {
                System.out.println("Too LOW! Try again.");
            } 
            else if (guess > secretNumber) {
                System.out.println("Too HIGH! Try again.");
            } 
            else {
                System.out.println("\n🎉 Congratulations!");
                System.out.println("You guessed the correct number!");
                System.out.println("Attempts: " + attempts);
            }

        } while (guess != secretNumber);

        scanner.close();
    }
}

        scanner.close();
    }
}
