# Ex12 Add Elements from an Array into a TreeSet
## DATE: 12-10-2025
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Read n and then read n integers into the array arr.
2. Call convertArrayToTreeSet and pass the array as input.
3. Inside the method, create an empty TreeSet to store elements in sorted order.
4. Traverse the array and insert each element into the TreeSet.
5. Return the TreeSet and print each element from it in ascending order.  

## Program:
```JAVA
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: Ashwin Akash M
RegisterNumber: 212223230024
*/
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        // Type Your Code Here.
        TreeSet<Integer> set1=new TreeSet<>();
        for(int num : arr)
        set1.add(num);
        
        return set1;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}

```

## Output:



## Result:
The program successfully adds elements from an array into a TreeSet.
