//Health application: BMI)

# Extra_Ex3_6

package com.personal.Extra3_6;

import java.util.Scanner;

public class Extra3_6 {

	public static void main(String[] args) {

		System.out.println("****** Calculating the BMI");

		Scanner sc= new Scanner(System.in);
		int weight,inch,feet;
		System.out.println("Enter your weight in pond");
		weight= sc.nextInt();
		System.out.println("Enter your height in inch");
		inch= sc.nextInt();
		System.out.println("Enter your feet");
		feet= sc.nextInt();
		
		double weightInKilos = weight * 0.453592;
        double heightInMeters = (((feet * 12) + inch) * .0254);
        double bmi = weightInKilos / Math.pow(heightInMeters, 2.0);
		
		if (bmi < 18.5 ) {
            System.out.print("Underweight");
        }

        else if (bmi >= 18.5 && bmi < 25) {
            System.out.print("Normal");
        }

        else if (bmi >= 25 && bmi < 30) {
            System.out.print("Overweight");
        }

        else if (bmi >= 30) {
            System.out.print("Obese");
        }
		
	}

}
