package MDemo;

import java.util.Scanner;

public class LargestElementFinder {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter numbers separated by spaces
        System.out.print("Enter numbers separated by spaces: ");
        String input = scanner.nextLine();

        // Split the input string by spaces to get individual number strings
        String[] numberStrings = input.split(" ");

        int[] numbers = new int[numberStrings.length];

        try {
            // Convert the number strings to integers
            for (int i = 0; i < numberStrings.length; i++) {
                numbers[i] = Integer.parseInt(numberStrings[i]);
            }

            // Call the function to find the largest element
            int largestElement = findLargest(numbers);

            // Print the result
            System.out.println("The largest element is: " + largestElement);

        } catch (NumberFormatException e) {
            System.out.println("Invalid input. Please enter valid integers separated by spaces.");
        }
    }

    // Function to find the largest element in an array of integers
    public static int findLargest(int[] numbers) {
        if (numbers.length == 0) {
            throw new IllegalArgumentException("Empty array, no largest element");
        }

        int largest = numbers[0];

        for (int i = 1; i < numbers.length; i++) {
            if (numbers[i] > largest) {
                largest = numbers[i];
            }
        }

        return largest;
    }
}
