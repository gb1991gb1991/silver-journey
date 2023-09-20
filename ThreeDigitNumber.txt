/**
 * 
 */
package packagename;
import java.util.Scanner; 

/**
 * 
 */
public class Classname {

	/**
	 * 
	 */
	public Classname() {
		// TODO Auto-generated constructor stub
	}

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		System.out.println("enter a three digit integer between 000 and 999");
		String input = scanner.nextLine();
		if ((input.length() == 3)  ){

			int number = Integer.parseInt(input);
			int firstDigit = number / 100 % 10;
			int SecondDigit= (number / 10) %10;
			int thirdDigit = number % 10;
			if (firstDigit + SecondDigit == thirdDigit) {
				System.out.println("the first two digits add up to the third digit");
			}
			if (firstDigit * SecondDigit == thirdDigit) {
				System.out.println("the first two digits multiply to the third digit");
			}
			if (firstDigit - SecondDigit == thirdDigit) {
				System.out.println("the first two digits subdract to the third digit");
			}
			if (firstDigit / SecondDigit == thirdDigit) {
				System.out.println("the first two digits divide to the third digit");
			}
			else {
				System.out.println("there are no remaining operator to match the third digit.");
			}

		}
		else {
			System.out.println("please enter a valid three digit integer.");
		}
		scanner.close();


	}


}
