import java.util.Scanner;

public class Student {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter name: ");
        String name = sc.nextLine();

        System.out.print("Enter age: ");
        int age = readInt(sc);

        System.out.print("Enter standard: ");
        String standard = sc.nextLine();

        System.out.print("Enter roll number: ");
        int rollNo = readInt(sc);

        System.out.println("\nStudent Details:");
        System.out.println("Name      : " + name);
        System.out.println("Age       : " + age);
        System.out.println("Standard  : " + standard);
        System.out.println("Roll No   : " + rollNo);

        sc.close();
    }

    // Helper to safely read an integer from the scanner
    private static int readInt(Scanner sc) {
        while (true) {
            String line = sc.nextLine().trim();
            try {
                return Integer.parseInt(line);
            } catch (NumberFormatException e) {
                System.out.print("Invalid number. Please enter again: ");
            }
        }
    }
}
# Java-programs
