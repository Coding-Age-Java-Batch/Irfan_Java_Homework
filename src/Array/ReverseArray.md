package Array;

import java.util.Scanner;
public class ReverseArray {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("enter size of array");
        int size=sc.nextInt();
        int[] arr = new int[size];
        for (int i=0; i<size; i++){
            arr[i]=sc.nextInt();
        }
        System.out.println("Original array - ");
        for (int i=0; i<size; i++){
            System.out.print(arr[i]+"  ");
        }
        System.out.println();
        int start = 0;
        int end = arr.length - 1;
        while (start < end) {
            int temp = arr[start];
            arr[start] = arr[end];
            arr[end] = temp;
            start++;
            end--;
        }
        System.out.println("Reversed Array:");
        for(int result : arr){
            System.out.print(result +"  ");
        }

    }

}

