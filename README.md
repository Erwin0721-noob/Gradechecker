import java.util.Scanner;

public class GradeChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter your grade (0-100): ");
        int grade = scanner.nextInt();
        
        if (grade >= 90 && grade <= 100) {
            System.out.println("Amazing you got A");
        } else if (grade >= 80 && grade < 90) {
            System.out.println("B");
        } else if (grade >= 70 && grade < 80) {
            System.out.println("C");
        } else if (grade >= 60 && grade < 70) {
            System.out.println("You got D");
        } else if (grade >= 0 && grade < 60) {
            System.out.println("F");
        } else {
            System.out.println("Invalid grade entered.");
        }
        
        scanner.close();
    }
}
