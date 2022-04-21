# ubiquitous-giggle
chat bot, first programm
import java.util.Scanner;

public class SimpleBot {
	final static Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {

        System.out.println("Hello! My name is Aid.");
        System.out.println("I was created in 2018.");
        System.out.println("Please, remind me your name.");

        String name = scanner.nextLine();

        System.out.println("What a great name you have, " + name + "!");
        System.out.println("Let me guess your age.");
        System.out.println("Enter remainders of dividing your age by 3, 5 and 7.");

        int remainder3 = scanner.nextInt();
        int remainder5 = scanner.nextInt();
        int remainder7 = scanner.nextInt();

        
        int age = (remainder3 * 70 + remainder5 * 21 + remainder7 * 15) % 105;
        System.out.println("Your age is " + age + "; that's a good time to start programming!");
        System.out.println("Now I will prove to you that I can count to any number you want.");

        // read a number and count to it here
        System.out.println("Please enter your number: ");
        
        int num = scanner.nextInt();
        
        for(int i = 0; i <= num; i++) {
        	System.out.println(i+ "!");
            //System.out.printf("%d!\n", i);
        }
        
        System.out.println("Completed, have a nice day!");
        test();
    }

    static void test() {
    	System.out.println("Let's test your programming knowledge.");
    	System.out.println("Why do we use methods?");
    	
    	String str1 = "1. To repeat a statement multiple times.";
    	String str2 = "2. To decompose a program into several small subroutines.";
    	String str3 = "3. To determine the execution time of a program.";
    	String str4 = "4. To interrupt the execution of a program.";
    	System.out.println(str1+ '\n' +str2+ '\n' +str3+ '\n' +str4);
    	
    	int antwort = scanner.nextInt();
    	
    	if (antwort != 2) {
    		System.out.println("Please, try again.");
    	} else {
    		end();
    	}

    }

    static void end() {
    	System.out.println("Congratulations, have a nice day!"); // Do not change this text
    }

}
