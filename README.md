package MDemo;
import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

public class EvenNumberFilter1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		//Create a Scanner object for user input
		Scanner sc=new Scanner(System.in);
		//Read the size of the array
		System.out.println("Enter the number of elements in the array:");
		int size=sc.nextInt();
		sc.nextInt();// Consume
		
		int[] numbers=new int[size];
		System.out.println("Enter the numbers");
		
		for(int i=0; i<size; i++) {
			numbers[i]=sc.nextInt();
		}
		sc.close();
		
		List<Integer>EvenNumber = new ArrayList<>();
		int sum =0;
		
		
		for(int number: numbers) {
			if (number %2==0) {
				EvenNumber.add(number);
				sum+=number;
			}
		}
			System.out.println("Even Numbers:");
			for(int evenNumber : EvenNumber) {
				System.out.println("evenNumbers:");
              }
		
			System.out.println("Sum of even numbers:" + sum);

	}

}
