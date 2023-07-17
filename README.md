import java. util.Scanner;
public class Main
{
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		int grade [] = new int [4];
		
		System.out.println("Input grades: ");
		grade[0] = sc.nextInt();
	    grade[1] = sc.nextInt();
		grade[2] = sc.nextInt();
		grade[3] = sc.nextInt();
		
		int ave = (grade[0]+grade[1]+grade[2]+grade[3])/4;
		
		System.out.println("\nAverage: "+ ave);
		
		if(ave > 100)System.out.println("You must be Einstein");
		else if (ave >= 98 && ave <= 100) System.out.println("With Highest Honors!");
		else if (ave >= 95 && ave <= 97) System.out.println("With High Honors!");
		else if (ave >= 90 && ave <= 94) System.out.println("With Honors!");
		else if (ave >= 75 && ave <= 89) System.out.println("Passed!");
		else if (ave < 75) System.out.println("Failed!");
		else System.out.println("Error!");
	}
}
