``java
import java.util.Scanner;
import javax.swing.JOptionPane;

public class InputExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = scanner.nextLine();
        System.out.println("Hello, " + name + "! Nice to meet you!");

        String ageInput = JOptionPane.showInputDialog("Enter your age: ");
        int age = Integer.parseInt(ageInput);
        JOptionPane.showMessageDialog(null, "You are " + age + " years old!");

        scanner.close();
    }
