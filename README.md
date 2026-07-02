//TASK 1:

import java.util.Scanner;

public class andersenTask {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        // Task 1 : for the task - if the entered number is greater than 7, then print "Hello"
        System.out.print("enter a number: ");
        int number = scanner.nextInt();

        if (number > 7) {
            System.out.println("Hello");
        }

        scanner.nextLine();

        // Task 2
        System.out.print("enter your name: ");
        String name = scanner.nextLine();

        if (name.equals("John")) {
            System.out.println("hello, John");
        } else {
            System.out.println("there is no such name");
        }

        // Task 3
        int[] numbers = {3, 2, 5, 9, 12, 43, 17, 21, 25, 30, 54, 122};

        System.out.println("numbers divisible by 3:");

        for (int num : numbers) {
            if (num % 3 == 0) {
                System.out.println(num);
            }
        }

        scanner.close();
    }
}
// TASK 2:
//Given the bracket sequence: [((())()(())]]
//1. Is this bracket sequence correct?
//Answer: No, it is not correct.

//2. What should be changed to make it correct?
//The sequence has one extra closing square bracket (]) at the end and is missing an opening square bracket ([) before the last part. A correct version is:

//[((())()(()))]

//This sequence is correct because every opening bracket has a matching closing bracket, and the brackets are properly nested.
