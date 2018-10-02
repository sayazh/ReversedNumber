# ReversedNumber
PalindromeNumber
package Assignments2;

import java.util.Scanner;

public class reversedNumbers {
	public static void main(String[] args) {

		System.out.println("Enter please any numbers");
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();

		int rev, num2 = 0, k = 0;
		while (num > 0) {
			rev = num % 10;
			num = num / 10;
			k = k * 10 + rev;
		}
		if (num2 == num) {
			System.out.println(k);
			System.out.println("This number is Palindrome");
		} else {
			System.out.println("This number is not Palindrome");
		}

		sc.close();
	}
}
