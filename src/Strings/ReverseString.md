package Strings;

import java.util.Scanner;
public class ReverseString {
    public  String reverse(String str) {
        String reversed = "";
        for (int i = str.length() - 1; i >= 0; i--) {
            reversed = reversed + str.charAt(i);
        }
        return reversed;
    }
    public static void main(String[] args) {
        ReverseString rs=new ReverseString();
        Scanner sc=new Scanner(System.in);
        System.out.println("enter a string");
        String input = sc.nextLine();
        String result = rs.reverse(input);
        System.out.println("Reversed String: " + result);
    }
}

