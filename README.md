// Java Program to print the duplicate elements of an array
import java.util.Arrays;
import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter the length of an Array");
        int n=sc.nextInt();
        int[] arr=new int[n];
        for(int i=0;i<n;i++){
           arr[i]=sc.nextInt();
        }
        
        System.out.println(Arrays.toString(arr));
        Arrays.sort(arr);
        System.out.println(Arrays.toString(arr));
        
        for(int i=0;i<arr.length;i++){
            for(int j=i+1;j<arr.length;j++){
              if(arr[i]==arr[j]){
                System.out.println("Duplicate elements in Array:" + arr[i]);
              }
            }
        }
        
    }
}
