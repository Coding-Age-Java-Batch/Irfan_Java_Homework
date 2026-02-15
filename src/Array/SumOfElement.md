package Array;

import java.util.Scanner;
class sumOfElement {
public static void main(String[] args) {
Scanner sc=new Scanner(System.in);
System.out.println("enter size of array");
int size= sc.nextInt();
int[] arr=new int[size];
System.out.println("enter array elements ");
for(int i=0; i<size; i++){
arr[i]=sc.nextInt();
}
int sum=0;
        for(int i=0; i<size; i++){
            sum=sum+arr[i];
        }
        System.out.println("Sum of array elements :- "+sum);

    }
}
