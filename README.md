import java.util.Scanner;
import java.util.Random;

public class NumberGuessingGame {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        Random random = new Random();

        int secretNumber = random.nextInt(100) + 1;
        int guess;
        int attempts = 0;

        System.out.println("================================");
        System.out.println("      NUMBER GUESSING GAME");
        System.out.println("================================");
        System.out.println("I have selected a number from 1 to 100.");
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
                System.out.println("Number of attempts: " + attempts);
            }

        } while (guess != secretNumber);

        scanner.close();
    }
}# -Number-Guessing-Game
