# Week-1
Introduction code
import java.util.ArrayList;
import java.util.Scanner;

class User {
    String name;
    String email;
    String password;

    User(String name, String email, String password) {
        this.name = name;
        this.email = email;
        this.password = password;
    }
}

public class Main {
    static Scanner sc = new Scanner(System.in);
    static ArrayList<User> users = new ArrayList<>();

    public static void main(String[] args) {
        register();
    }

    static void register() {
        System.out.println("===== RakshanaMart ONLINE SHOPPING =====");
        System.out.println("===== REGISTER =====");

        System.out.print("Enter Name: ");
        String name = sc.nextLine();

        System.out.print("Enter Email: ");
        String email = sc.nextLine();

        System.out.print("Enter Password: ");
        String password = sc.nextLine();

        users.add(new User(name, email, password));

        System.out.println("Registration Successful!");
    }
}
