Hangman.java
import java.util.Scanner;

public class HangmanGame {
   
    private static final String WORD = "hangman";

   
    private static final int MAX_MISSES = 6;

   
    private static String guessedLetters;
    private static int numMisses;

    public static void main(String[] args) {
      
        guessedLetters = "";
        numMisses = 0;

       
        Scanner scanner = new Scanner(System.in)) {
           
            while (!isGameOver()) {
                
                System.out.println("Word: " + getHiddenWord());
                System.out.println("Guessed letters: " + guessedLetters);
                System.out.println("Misses left: " + (MAX_MISSES - numMisses));
                System.out.print("Guess a letter: ");

               
                String guess = scanner.nextLine().toLowerCase();

              
                if (!isValidGuess(guess)) {
                    System.out.println("Invalid guess, please try again.");
                    continue;
                }

            
    }
}
