package Strings;


import java.util.Scanner;

public class PalindromCheck {
public static boolean isPalindrome(String str){
String org=str;
String reverse="";
for(int i=str.length()-1; i>=0; i--){
reverse= reverse+str.charAt(i);
}
return org.equals(reverse);
}
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("enter a string");
        String input= sc.nextLine();
        boolean result = isPalindrome(input);
        System.out.println(result);

    }
}
