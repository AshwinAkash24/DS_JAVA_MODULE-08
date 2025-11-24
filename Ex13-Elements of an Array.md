# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE: 12-10-2025
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Read the value that will be used to fill the array.
2. Call fillArray with size 10 and the given value.
3. Inside fillArray, create an integer array of the specified size.
4. Use Arrays.fill to store the given value in every position of the array.
5. Return the filled array and print all its elements.
  

## Program:
```JAVA
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: Ashwin Akash M
RegisterNumber: 212223230024
*/
import java.util.*;

public class FillArrayUsingArraysFill {

    public static int[] fillArray(int size, int value) {
        // Type Your Code Here.
        int arr[]=new int[size];
        Arrays.fill(arr,value);
        return arr;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

```

## Output:



## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
